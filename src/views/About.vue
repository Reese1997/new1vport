<template>

<section>
  <div class="row">
    <div class="col-md-6 col-sm-12" id="aboutimage">
      <img src="../assets/images/reese/Reese4.jpg" style="height: 80vh;">
    </div>

    <div class="col-md-6 col-sm-12" id="aboutparagraph">
      <p style="font-size: 60px; font-family: 'Poppins', serif; color: #666666;">ABOUT</p>
      <p>Me</p>
      <p style="font-family: 'Poppins', serif; font-size: 20px;">
        Hi, I'm Reese Simone Abrahams! <br><br> I specialise as a Full-Stack Developer.<br><br>
        With functionality, I construct and transform code into beautiful applications. My skills range from a wide variety of coding niches, from databases, graphic design to UI/UX management, and I do my job pretty well. <br/><br/>
     </p>
    </div>
  </div>

</section>

  

</template>

<script>
export default {};
</script>

<style scoped>

@media screen and (max-width: 585px) {
    #aboutparagraph{ 
      padding: none;
      }
}

@media screen and (max-width: 600px) {

  section{
    height: 190vh;
  }
}

@media screen and (max-width: 767px) {
  #aboutparagraph{ 
    padding-left: 180px;
  }
}

@media only screen and (max-width: 900px) {
  .masthead {
    padding: 7em 0;
  }
  .masthead-heading {
    font-size: 3em;
  }
}

#aboutparagraph {
  padding-right: 180px
}

body {
  /* Typography Declarations */
  color: #030303;
  font-size: 1em;
  font-family: 'Poppins', sans-serif;
  background-color: white;
}
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');



html, body {
  background-color: red;
}
p {
  font-family: 'Poppins', serif;
  color: #323232;
  letter-spacing: 2px;
  font-size: 60px;
}
img {
  height: 100%;
  border-right-style: solid;
  border-right-width: 5px;
  border-right-color: #C5964B;
}
.fa-bars {
  font-size: 25px;
  color: #4c4c4c;
  cursor: pointer;
}
.fa {
  color: #4c4c4c;
}
.menu-container {
  position: absolute;
  left: 40px;
  top: 30px;
}
.image-container {
  height: 100%;
  margin-left: 100px;
  position: absolute;
}
.text-container {
  height: 100%;
  width: 400px;
  position: absolute;
  left: 510px;
}
.nav-bar {
  margin: auto;
  position: absolute;
  top: 30px;
  left: 0;
  right: 0;
  height: 30px;
  width: 300px;
}
.underline {
  margin: auto;
  position: absolute;
  top: 60px;
  left: 0;
  right: -47px;
  height: 1px;
  width: 54px;
  background-color: #C5964B;
}
.underline2 {
  margin: auto;
  position: absolute;
  top: 309px;
  left: 50px;
  height: 1.2px;
  width: 87px;
  background-color: #C5964B;
}
.sub-title {
  position: absolute;
  height: 100px;
  width: 300px;
  top: 210px;
  bottom: 0;
  left: 50px;
}
.title-container {
  position: absolute;
  height: 100px;
  width: 300px;
  top: 170px;
  bottom: 0;
  left: 45px;
}
.fa-caret-down {
  position: absolute;
  margin: auto;
  top: 4px;
  bottom: 0;
  text-align: center;
  font-size: 14px;
  width: 20px;
  height: 20px;
}
.dropdown {
  position: absolute;
  margin: auto;
  top: 0;
  bottom: 50px;
  left: -80px;
  right: 0;
  width: 20px;
  height: 20px;
  border-style: solid;
  border-width: 1px;
  cursor: pointer;
}
.p-container {
  font-family: 'Poppins', serif;
  font-size: 15px;
  margin: auto; 
  position: absolute;
  bottom: 80px;
  left: 0;
  right: 0;
  height: 200px;
  width: 400px;
}
.container {
  position: absolute;
  margin: auto;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: #FCFCFD;
  width: 900px;
  height: 600px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
.background {
  position: absolute;
  margin: auto;
  top: 0;
  bottom: 0;
  left: 0;
  background-color: #0e0431;
  height: 70%;
  width: 25%;
  border-right-style: solid;
  border-right-width: 5px;
  border-right-color: #C5964B;
}
</style>
