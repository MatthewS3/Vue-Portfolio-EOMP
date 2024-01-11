<template>
  <div class="about">
    <h1>About Me:</h1>
  </div>
  <div class="body">
    <div class="container1">
      <div class="row">
        <div class="left-side">
          <div class="wrapper">
            <div class="typing-demo">Hi I'm <span class="name">Matthew Swain...</span></div>
          </div>
        </div>
        <div class="right-side">
          <div class="about-img">
            <img src="https://i.postimg.cc/pVzTvjMY/Screenshot-2024-01-08-150841.png" />
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="quote-of-me">
    <p class="about-me">
      Against all odds, I have as emerged as a resilient and tenacious individual who has
      navigated through numerous challenges on the path to becoming a Web/Software
      developer.
      <br /><br />
      <span class="q1">
        From facing financial constraints to overcoming educational barriers, ive
        demonstrated unwavering determination and an unyielding spirit. The journey has
        been marked by sleepless nights spent mastering coding languages, countless
        setbacks that only fueled the desire to succeed, and a relentless pursuit of
        knowledge.
      </span>
      <br /><br />
      My passion for programming begun at a later stage in my life and i can say ive found
      my passion and calling in this field. Throughout high school my mind was set on
      becoming a Graphic Designer and an architech but that never came to fruition. The
      year of 2023 was the turning point in my life and have deicated my all into becoming
      a developer and i can say ive made the right choices.
      <br /><br />
      <span class="q2">
        Through perseverance, ive transformed obstacles into stepping stones, setbacks
        into comebacks and setbacks into setups for success defying expectations and
        proving that passion and dedication can triumph over any obsticle. From being
        pressured and influenced that i would become nothing and would not succeed in
        life.
      </span>
      <br /><br />
      Today, as I continue to evolve as a Developer, from having nothing to have everthing
      i need to suceed I can stand as a individual that serves as an inspiration to
      others, showcasing the incredible heights that can be reached when one refuses to be
      defined by their challenges.
    </p>
  </div>
  <div class="container2">
    <div class="box">
      <div class="box-img">
        <img src="fam.jpg" />
      </div>
      <div class="box-text">
        <h2>About My Family</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
          incididunt ut labore et dolore magna aliqua...
        </p>
        <a href="#">view more</a>
      </div>
    </div>
    <div class="box">
      <div class="box-img">
        <img src="prof2.jpg" />
      </div>
      <div class="box-text">
        <h2>Some of My Story</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
          incididunt ut labore et dolore magna aliqu...
        </p>
        <a href="#">view more</a>
      </div>
    </div>
    <div class="box">
      <div class="box-img">
        <img src="it.jpg" />
      </div>
      <div class="box-text">
        <h2>Future Aspirations</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
          incididunt ut labore et dolore magna aliqua...
        </p>
        <a href="#">view more</a>
      </div>
    </div>
  </div>
</template>

<script></script>

<style>
.body {
  width: 95%;
  height: 600px;
  background-image: url(https://i.postimg.cc/HsBNKSnJ/Screenshot-2024-01-08-144001.png);
  display: flex;
  margin: 80px auto;
}

.right-side {
  display: flex;
  float: left;
  width: 50%;
  padding: 20px;
  height: 300px;
}

.right-side .about-img {
  position: absolute;
  top: 300px;
  left: 1000px;
}

.about-img:hover {
  transform: scale(1.1);
  transition: 2s ease-in-out;
  background: #3d3f3f;
  box-shadow: 2px 2px 2px #000;
  z-index: 2;
}

.about-img::before {
  position: absolute;
  content: "";
  right: -30px;
  top: 15px;
  border: 10px solid rgba(31, 30, 30, 0.5);
  width: 100%;
  height: 100%;
}

.about-img img {
  height: 450px;
  width: 100%;
}

.about-me {
  font-size: 15px;
}

.name {
  color: gold;
}

.left-side {
  display: flex;
  margin-top: 30px;
  float: left;
  width: 100%;
  padding: 60px;
  height: 400px;
}

.wrapper {
  height: 400px;
  display: grid;
  place-items: center;
}

.typing-demo {
  width: 500px;
  animation: typing 4s steps(22), blink .5s step-end infinite alternate;
  white-space: nowrap;
  overflow: hidden;
  border-right: 3px solid;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 3em;
}

@keyframes typing {
  from {
    width: 0
  }
}
    
@keyframes blink {
  50% {
    border-color: transparent
  }
}

.quote-of-me {
  width: 1000px;
  height: 340px;
  display: block;
  background-color: #333;
  border-radius: 10px;
}

.q1 {
  color: gold;
}

.q2 {
  color: gold;
}

.container2 {
  width: 95%;
  height: auto;
  padding: 10px;
  margin: 80px auto;
  display: flex;
  justify-content: center;
}

.box {
  width: 380px;
  height: 700px;
  background: gold;
  margin: 0px 10px;
  transition: 2s;
}

.box:hover {
  transform: scale(1.1);
  background: goldenrod;
  box-shadow: 2px 2px 2px #000;
  z-index: 2;
}

.box-img img {
  height: 110px;
  width: 110px;
  background-size: cover;
  background-position: center;
  border-radius: 50px;
  transform: translate(-50%, -50%);
  position: relative;
  margin-top: 30%;
  margin-left: 50%;
}

.box-text {
  padding: 10px;
  margin: 5px;
}

.box-text h2 {
  font-size: 20px;
  margin-left: 25%;
  margin-bottom: 30px;
  color: black;
}

.box-text p {
  line-height: 22px;
  font-size: 16px;
  margin-left: 20px;
  margin-bottom: 12px;
  color: black;
}

.box-text a {
  background: rgb(219, 170, 178);
  color: #000;
  padding: 7px 15px;
  display: inline-block;
  text-decoration: none;
  text-transform: capitalize;
  position: relative;
  margin-top: 10%;
  margin-left: 35%;
}

.box-text a:hover {
  background-color: rgb(238, 117, 137);
  color: whitesmoke;
  font: bold;
}
</style>
