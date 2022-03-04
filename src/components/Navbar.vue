<template>
  <nav id="nav" :class="{ active: isActive }">
     <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
    <router-link to="/work">Work</router-link>
    <router-link to="/skills">Skills</router-link>
    <router-link to="/projects">Projects</router-link>
    <router-link to="/testimonials">Testimonials</router-link>
    <router-link to="/contact">Contact</router-link>
  </nav>
  <button id="nav-btn" @click="toggleNav">
    <i className="fas fa-bars"></i>
  </button>
</template>
<script>
export default {
  data() {
    return {
      isActive: false,
    };
  },
  methods: {
    toggleNav() {
      this.isActive = !this.isActive;
    },
    logout() {
      localStorage.clear();
      this.toggleNav;
    },
  },
};
</script>
<style lang="scss" scoped>

#nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background: rgb(41, 47, 53);
  z-index: 200;
}

#nav-btn {
  position: fixed;
  top: 20px;
  right: 20px;
  background: #f5f5f5;
  box-shadow: 8px 8px 15px #e4e4e4, -8px -8px 15px #ffffff;
  padding: 20px;
  border-radius: 50%;
  border: none;
  outline: none;
  display: none;
  z-index: 201;

}
#nav {
  padding: 30px;

  a {
     font-size: 20px;
  color: #eee2e2;
  text-decoration: rgb(15, 14, 15);
  padding: 9px;
  border-radius: 4px;
    &.router-link-exact-active:not(.logout) {
      color: white;
        background: rgb(21, 107, 192);
    }
  }
}

.fa-bars:before {
  color: red;
}

@media screen and (max-width: 628px) {
  #nav {
    height: 100%;
    left: -100vw;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    transition: left 0.1s linear;
  }
  #nav.active {
    left: 0;
  }
  #nav-btn {
    display: block;
  }
}

</style>
