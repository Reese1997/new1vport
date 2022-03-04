<template>
  <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/all.css" integrity="sha384-50oBUHEmvpQ+1lW4y57PTFmhCaXp0ML5d60M1M7uH2+nqUivzIebhndOJK28anvf" crossorigin="anonymous" />

<link href="https://fonts.googleapis.com/css?family=Poppins:200i,300,400&display=swap" rel="stylesheet" />

<footer id="contact">
  <ul>
    <div id="icon-container">
      <a href="https://www.linkedin.com/in/reese-abrahams-19525415b/">
        <div class="icon">
          <li><i class="fab fa-linkedin"></i></li>
        </div>
      </a>
    <a href="https://codepen.io/reese1997">
        <div class="icon">
          <li><i class="fab fa-codepen"></i></li>
        </div>
      </a>
      <a href="https://reeseabrahams1997@icloud.com">
        <div class="icon">
          <li><i class="far fa-envelope"></i></li>
        </div>
      </a>
      <a href="https://github.com/Reese1997">
        <div class="icon">
          <li><i class="fab fa-github"></i></li>
        </div>
      </a>
    </div>
  </ul>
  <p>&copy; 2021-2022, Made by Reese Abrahams</p>
</footer>
    <!-- Copyright -->
</template>


<script>
  import { MDBFooter, MDBContainer, MDBRow, MDBCol, MDBBtn } from 'mdb-vue-ui-kit';
  export default {
    components: {
      MDBFooter,
      MDBContainer,
      MDBRow,
      MDBCol,
      MDBBtn
    },
  };
</script>


<style>
body {
  margin: 0;
  padding: 0;
  font-family: "Poppins", sans-serif;
}

/* footer {
  position: absolute;
  width: 100%;
  bottom: 0;
} */

ul {
  margin: 0;
  padding: 0;
}

ul li {
  list-style: none;
}

#contact a {
  color: rgb(15, 112, 202);
  margin: 10px;
}

#contact {
  color: #fff;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 200px;
  background-color: rgb(41, 47, 53);
}

.icon {
  background-color: #fff;
  border-radius: 50%;
  width: 40px;
  height: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: transform 1s, box-shadow 0.5s;
  box-shadow: 0 2px 3px rgb(0 0 0 / 12%), 0 2px 2px rgb(0 0 0 / 24%);
}

#icon-container {
  display: flex;
  justify-content: center;
}

.icon:hover {
  transform: translateY(-3px);
  box-shadow: 0 3px 5px 5px rgb(0 0 0 / 12%), 0 3px 5px rgb(0 0 0 / 24%);
}

#contact p {
    font-size: 14px;
}

@media screen and (max-width: 426px) {
 #icon {
   width: 30px;
   height: 30px;
  }
  
  ul li {
    font-size: 12px;
  }
  
  #contact p {
    font-size: 10px;
  }
}

@media screen and (min-width: 2560px) {
 #icon {
   width: 50px;
   height: 50px;
  }
  
  ul li {
    font-size: 20px;
  }
  
  #contact p {
    font-size: 16px;
  }
}
</style>