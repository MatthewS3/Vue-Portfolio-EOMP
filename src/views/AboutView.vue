<template>
  <div class="body">
    <div class="container1">
      <div class="row">
        <div class="left-side">
          <div class="wrapper">
            <div class="typing-demo">
              Hi I'm <span class="name">Matthew Swain...</span>
            </div>
          </div>
        </div>
        <div class="right-side">
          <div class="about-img">
            <img src="https://i.postimg.cc/Kjr4KPD1/1000025645.jpg" />
          </div>
        </div>
      </div>
    </div>
  </div>
  <br>
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
      From being in a place where i was resulting to nothing not knowing what the future
      held for me. Being at a point where i was at home jobless and being rejected
      numerous times at both colleges and Universities I rose to the occation and made my
      own path toward becoming a web developer as saw a opportunity at life choices add
      grasped my opportunity with all my strenght and power and it has changed my life so
      much.
      <br /><br />
      <span class="q3">
        Today, as I continue to evolve as a Developer, from having nothing to have
        everthing i need to suceed I can stand as a individual that serves as an
        inspiration to others, showcasing the incredible heights that can be reached when
        one refuses to be defined by their challenges.
      </span>
    </p>
  </div>
</template>

<script></script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&display=swap');

.body {
  width: auto;
  height: 610px;
  background-image: url(https://i.postimg.cc/HsBNKSnJ/Screenshot-2024-01-08-144001.png);
  display: flex;
  padding: 65px;
}

.right-side {
  display: flex;
  float: left;
  width: 50%;
  padding: 0px;
  height: 300px;
}

.right-side .about-img {
  position: absolute;
  top: 190px;
  left: 1000px;
  animation: enlarge 5s infinite alternate; /* Animation properties */
}

@keyframes enlarge {
  0% {
    transform: scale(1); /* Initial size */
  }
  100% {
    transform: scale(1.15); /* Enlarged size */
  }
}

.about-img::before {
  position: absolute;
  content: "";
  right: -10px;
  top: -10px;
  border: 10px solid gold;
  width: 100%;
  height: 100%;
  border-radius: 10px;
}

.about-img img {
  height: 450px;
  width: 100%;
  border-radius: 10px;
  box-shadow: 0 5px 200px black;

}

.about-me {
  font-size: 16px;
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
  width: auto;
  animation: typing 5s steps(22), blink 0.5s step-end infinite alternate;
  white-space: nowrap;
  overflow: hidden;
  border-right: 3px solid;
  font-family: "Playfair Display", serif;
  font-size: 3em;
}

@keyframes typing {
  from {
    width: 0;
  }
}

@keyframes blink {
  50% {
    border-color: transparent;
  }
}

.quote-of-me {
  padding: 10px;
  height: 400px;
  display: block;
}

.q1 {
  color: gold;
}

.q2 {
  color: gold;
}

.q3 {
  color: gold;
}


</style>
