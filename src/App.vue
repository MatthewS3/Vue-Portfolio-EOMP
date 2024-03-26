<template>
  <NavBar />
    <router-view />
  <FooterView />
</template>
<script>
import NavBar from './components/NavBar.vue';
import FooterView from './components/FooterView.vue';

export default {
  components: {
    NavBar,
    FooterView,
  },
};
</script>

<style>
#app {
  font-family: "Playfair Display", serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ddd;
  animation: fadeIn 5s;
  background-color: black;
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
