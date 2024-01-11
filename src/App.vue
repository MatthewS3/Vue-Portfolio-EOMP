<template>
  <NavBar />
  <div class="home">
    <router-view />
  </div>
  <Footer />
</template>
<script>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    NavBar,
    Footer,
  },
};
</script>

<style>
body {
  background-color: #444;
}

#app {
  font-family: "Courier New", Courier, monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ddd;
  animation: fadeIn 5s;
}

nav {
  padding: 30px;
  font-size: 20px;
  text-decoration: none;
}

nav a:hover {
  color: gold;
  transition: 1.5s;
}

nav a {
  font-weight: bold;
  color: black;
  animation: fadeIn 5s;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

nav a.router-link-exact-active {
  color: gold;
}
</style>
