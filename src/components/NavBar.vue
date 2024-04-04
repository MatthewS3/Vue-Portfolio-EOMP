<template>
  <nav id="NAV">
    <a href="/">Home</a> |
     <a href="#About">About</a> |
    <a href="#Resume">Resume & Skills</a> |
    <a href="#Projects">Projects</a> |
    <a href="#Testimonials">Peer Reviews</a> |
    <a href="#Contact">Contact</a>
  </nav>
</template>

<script>
export default {};
</script>

<style>
#NAV {
  position: fixed; /* Make the navigation bar fixed */
  top: 0; /* Position it at the top of the viewport */
  width: 100%; /* Full width */
  background-color: gold; /* Example background color */
  /* Add some padding for spacing */
  z-index: 1000; /* Ensure it's on top of other content */
}

#NAV a {
  /* Add some spacing between links */
  text-decoration: none; /* Remove underline */
  color: #000; /* Link color */
}

/* Mobile styles */
@media (max-width: 768px) {
  .toggle-btn {
    display: block;
    position: absolute;
    top: 15px;
    left: 15px;
  }

  #NAV {
    width: 100% !important;
    font-size: 10px !important;
  }
}
</style>
