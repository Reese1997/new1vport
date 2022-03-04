<template>
  <Navbar />
  <router-view/>
</template>

<script>
import Navbar from "./components/Navbar.vue";
export default {
  components: { Navbar },
};
</script>

<style>

@import url("https://fonts.googleapis.com/css2?family=Nunito:wght@200;300;400;500;600;700;800;900&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Nunito", sans-serif;
}

main {
  background: #f5f5f5;
  min-height: 100vh;
  padding: 20px;
  padding-top: 100px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}





/* #app {
    font-family: 'Poppins', sans-serif;
    -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #f1e3e3;
}

#nav {
    font-family: 'Poppins', sans-serif;
  padding: 23px;
  background-color: rgb(41, 47, 53);
  bottom: 0;
  width: 100%;
}

#nav a {
  font-size: 20px;
  color: #eee2e2;
  text-decoration: rgb(15, 14, 15);
  padding: 9px;
  border-radius: 4px;
}

#nav a.router-link-exact-active {
  color: white;
  background: rgb(21, 107, 192);
  
}
button {
  margin: 0 10px;
  padding: 10px;
  border: none;
  border-radius: 4px;
} */


</style>
