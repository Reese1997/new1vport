<template>
  <!-- <img src="@/assets/bgblck.jpg" alt="" /> -->
  <div class="background animate__animated animate__zoomIn">

    <div class="content">
      <h1>Reese Simone Abrahams</h1>
    <h2>I am <span id="text"></span></h2>

    <!-- Social Media -->
    <div class="social-media">

    <a
      href="https://codepen.io/reese1997 /"
      class="fab fa-codepen"
      target="_blank"
      style="font-size: 70px; color: #222"
    ></a>
    <a
      href="https://github.com/Reese1997/"
      class="fab fa-github"
      style="font-size: 70px; color: #222"
    ></a>
    <a
      href="https://www.linkedin.com/in/reese-abrahams-19525415b/"
      class="fa fa-linkedin"
    ></a>
    </div>

    </div>
 
  </div>

</template>

<script>
export default {};
const sentences = [
  "Reese",
  "Front-End Developer",
  "Software Developer",
  "Creative and logical",
];

function waitForMs(ms) {
  return new Promise((resolve) => setTimeout(resolve, ms));
}

async function typeSentence(sentence, element, delay = 100) {
  const letters = sentence.split("");
  let i = 0;
  while (i < letters.length) {
    await waitForMs(delay);
    document.querySelector(element).append(letters[i]);
    i++;
  }
}

async function deleteSentence(element) {
  const sentence = document.querySelector(element).innerHTML;
  const letters = sentence.split("");
  while (letters.length > 0) {
    await waitForMs(100);
    letters.pop();
    document.querySelector(element).innerHTML = letters.join("");
  }
}

async function sentenceLoop(sentenceList, element) {
  let i = 0;
  while (true) {
    await typeSentence(sentenceList[i], element);
    await waitForMs(1500);
    await deleteSentence(element);
    await waitForMs(500);
    i++;
    if (i >= sentenceList.length) {
      i = 0;
    }
  }
}

sentenceLoop(sentences, "#text");

</script>

<style scoped>

body {
  margin: 0;
  padding: 0;
}

.background {
  background-image: url("../assets/images/background_images/aboutr.jpeg");
  background-size: 300px 300px;
  height: 100vh;
  width: 100%;
  background-position: fixed;
  background-size: cover;
  background-repeat: none;
  z-index: 199;
}

.content {
  padding-top: 400px;
  backdrop-filter: blur(4px) brightness(60%);
  z-index: 2;
  height: 100vh;
  text-align: center;
}

.home {
  padding: 90px;
  border-radius: 10px;
  cursor: pointer;
  color: rgb(14, 13, 13);
}

h1 {
  color: rgb(245, 245, 253);
  font-size: 60px;
}
h2 {
  text-align: center;
  color: rgb(255, 247, 247);
  font-size: 50px;
}

#text:after {
  width: 3px;
  height: 100%;
  background: black;
  position: absolute;
  animation: blink 1s infinite;
}

@keyframes blink {
  0%,
  49% {
    background: rgb(252, 248, 248);
  }
  50%,
  100% {
    background: rgb(255, 252, 252);
  }
}

</style>
