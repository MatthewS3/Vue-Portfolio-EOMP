<template>
  <div class="About">
    <h1>About Me</h1>
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
    <div class="caart">
      <div class="card25">
        <div class="content">
          <p class="heading">The Story Of Matthew :</p>
          <p class="about-me">
            Against all odds, I have emerged as resilient and tenacious
            individual who has navigated through numerous challenges on the path
            to becoming a web/software developer.
            <br /><br />
            <span class="q1">
              From facing financial constraints to overcoming educational
              barriers, I have demonstrated unwavering determination and an
              unyielding spirit. The journey has been marked by sleepless nights
              spent mastering coding languages, countless setbacks that only
              fueled the desire to succeed and a relentless pursuit of
              knowledge.
            </span>
            <br /><br />
            My passion for programming began at a later stage in my life, and I
            can say I have found my passion and calling in this field.
            Throughout high school, my mind was set on becoming a graphic
            designer, a coder aswell as an architect, but that never came to
            fruition. The year 2023 was the turning point in my life and have
            deicated my all into becoming a developer. and I can say I made the
            right choices.
            <br /><br />
            <span class="q2">
              Through perseverance, I transformed obstacles into stepping
              stones, setbacks into comebacks, and setbacks into setups for
              success. Defying expectations and proving that passion and
              dedication can triumph over any obsticle. From being pressured and
              influenced into thinking i would become nothing and would not
              succeed in life.
            </span>
            <br /><br />
            From being in a place where I was resulting to nothing, not knowing
            what the future held for me. I was at a point where I was at home,
            jobless and being rejected numerous times at both colleges and
            Universities I rose to the occasion and made my own path toward it.
            becoming a coder / developer as I saw an opportunity at Life Choices
            Academy. I grasped my opportunity with all my strength and power,
            and it has changed my life so much.
            <br /><br />
            <span class="q3">
              Today, as I continue to evolve as a Developer, from having nothing
              to have everthing i need to succeed I can stand as a individual
              that serves as an inspiration to others, showcasing the incredible
              heights that can be reached when one refuses to be defined by
              their challenges.
            </span>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script></script>

<style scope>
@import url("https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&display=swap");

.container1 {
  width: auto;
  height: 610px;
  background-image: url(https://i.postimg.cc/HsBNKSnJ/Screenshot-2024-01-08-144001.png);
  display: flex;
  border-radius: 70px;
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
  top: 780px;
  left: 1000px;
  width: 300px; /* Set your desired initial width */
  animation: enlarge 5s infinite alternate ; /* Animation properties */
}

@keyframes enlarge {
  0% {
    transform: scale(1.05); /* Initial size */
  }
  100% {
    transform: scale(1.15); /* Enlarged size */
  }
}

.about-img::before {
  position: absolute;
  content: "";
  right: -10px;
  border: 10px solid gold;
  width: 100%;
  height: 490px;
}

.about-img img {
  height: 500px;
  width: 100%;
}

.about-me {
  font-size: 20px;
  font-family: "Playfair Display", serif;
}

.name {
  color: gold;
}

.left-side {
  display: flex;
  margin-top: 30px;
  float: left;
  width: 600px;
  padding: 60px;
  height: 400px;
}

.wrapper {
  height: 400px;
  display: grid;
  place-items: center;
}

.typing-demo {
  width: 510px;
  animation: typing 4s steps(22), blink 0.5s step-end infinite alternate;
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

.q1 {
  color: gold;
  font-size: 20px;
}

.q2 {
  color: gold;
  font-size: 20px;
}

.q3 {
  color: gold;
  font-size: 20px;
}
/* ============CRDDDS================= */

.card25 {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 1100px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
  padding: 32px;
  overflow: hidden;
  border-radius: 70px;
  background: #212121;
  border: 4px solid Gold;
  transition: all 0.6s cubic-bezier(0.23, 1, 0.32, 1);
}

.caart {
  margin-left: 160px;
  margin-top: 100px;
}

.content .heading {
  font-weight: 700;
  font-size: 32px;
  font-family: "Playfair Display", serif;
}

.content p {
  line-height: 1.6;
  font-family: "Playfair Display", serif;
}

.card25:hover {
  box-shadow: 0 5px 50px gold;
  border-color: gold;
  transform: scale(1.1);
}
</style>
