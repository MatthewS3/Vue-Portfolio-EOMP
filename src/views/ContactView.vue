<template>
<h1>Contact Me:</h1>
  <div class="contact">
    <div id="square">
      <div id="image"></div>
      <div id="info">
        <h1>First Last</h1>
        <p>[c] (123) 456-7890</p>
        <p>[o] (098) 765-4321</p>
        <p>[e] email@example.com</p>
        <p>[w] www.example.com</p>
      </div>
    </div>
  </div>
</template>

<script>
</script>

<style>
.contact {
  margin-top: 200px;
}

#square {
  position: relative;
  height: 70px;
  width: 70px;
  left: 50%;
  background-color: white;
  transform: translate(-50%, -50%);
  border: black 2px solid;
  -webkit-animation: squareAppear 1 10s ease-out forwards;
  -moz-animation: squareAppear 1 10s ease-out forwards;
  -o-animation: squareAppear 1 10s ease-out forwards;
  animation: squareAppear 1 10s ease-out forwards;
  box-shadow: 5px 5px 5px 5px gold;
}

#image {
  opacity: 0;
  border-right: 1px solid black;
  height: 300px;
  width: 300px;
  float: left;
  -webkit-animation: imageAppear 1 1s ease-in-out forwards;
  -moz-animation: imageAppear 1 1s ease-in-out forwards;
  -o-animation: imageAppear 1 1s ease-in-out forwards;
  animation: imageAppear 1 1s ease-in-out forwards;
  animation-delay: 3s;
  background-image: url("https://i.imgur.com/vrSdt2B.jpg");
  background-size: cover;
}

#info {
  width: 399px;
  height: 300px;
  text-align: center;
  color: white;
  opacity: 0;
  float: right;
  animation: imageAppear 3s ease-in-out forwards;
  -moz-animation: imageAppear 3s ease-in-out forwards;
  -o-animation: imageAppear 3s ease-in-out forwards;
  animation: imageAppear 3s ease-in-out forwards;
  animation-delay: 3.5s;
}

p {
  font-size: 1.5em;
  font-weight: 100;
  margin: 0;
}

h1 {
  margin-top: 50px;
  text-shadow: 1px 2px gold;
  color: #111;
}

@keyframes squareAppear {
  0% {
    width: 50px;
    height: 50px;
    opacity: 0;
  }
  10% {
    width: 50px;
    height: 50px;
    opacity: 1;
    background-color: white;
  }
  20% {
    width: 700px;
    height: 300px;
    background-color: white;
  }
  30% {
    background-color: transparent;
  }
  100% {
    width: 700px;
    height: 300px;
    opacity: 1;
    background-color: transparent;
  }
}

@keyframes imageAppear {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
</style>
