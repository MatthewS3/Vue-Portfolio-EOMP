<template>
  <nav>
  <div class="navbar-toggle" onclick="toggleMenu()">
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
  </div>
  <div class="navbar-links" id="navbar-links">
    <a href="/">Home</a>
    <a href="#About">About</a>
    <a href="#Resume">Resume & Skills</a>
    <a href="#Projects">Projects</a>
    <a href="#Testimonials">Peer Reviews</a>
    <a href="#Contact">Contact</a>
  </div>
</nav>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    }
  }
};
</script>

<style>
nav {
  display: flex;
  position: fixed;
  justify-content: space-between;
  align-items: center;
  width: 95%;
  padding: 20px 20px;
  background-color: gold;
  color: #000;
  font-weight: bold;
  z-index: 30;
}

.navbar-toggle {
  display: none;
  flex-direction: column;
  cursor: pointer;
}

.bar {
  width: 25px;
  height: 3px;
  background-color: #000;
  margin: 3px 0;
}

.navbar-links {
  display: flex;
}

.navbar-links a {
  color: #111;
  text-decoration: none;
  letter-spacing: 4px;
  padding: 0 15px;
  
}

@media screen and (max-width: 768px) {
  .navbar-links {
    display: none;
    flex-direction: column;
    width: 100%;
    text-align: center;
    position: absolute;
    top: 60px; /* Adjust this value to suit your design */
    left: 0;
    background-color: #333;
  }

  .navbar-links.show {
    display: flex;
  }

  .navbar-toggle {
    display: flex;
  }
}
</style>
