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
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&display=swap');

body {
  background-color: #111;
}

#app {
  font-family: "Playfair Display", serif;
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
  letter-spacing: 5px;
}

nav a:hover {
  color: gold;
  transition: 1.5s;
}

nav a {
  font-weight: bold;
  color: #ddd;
  animation: fadeIn 5s;
  text-decoration: none;
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
