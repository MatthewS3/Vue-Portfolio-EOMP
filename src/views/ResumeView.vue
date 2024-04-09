<template>
  <br />
  <div id="Resume">
    <h1>My Skills:</h1>
    <div class="skills-container1">
      <div class="skill">
        <i class="fa-brands fa-html5"></i>
        <span>HTML5</span>
      </div>
      <div class="skill">
        <i class="fa-brands fa-css3-alt"></i>
        <span>CSS3</span>
      </div>
      <div class="skill">
        <i class="fa-brands fa-bootstrap"></i>
        <span>Bootstrap</span>
      </div>
      <div class="skill">
        <i class="fa-brands fa-js"></i>
        <span>JavaScript</span>
      </div>
    </div>
    <div class="skills-container2">
      <div class="skill">
        <i class="fa-brands fa-vuejs"></i>
        <span>Vue.js</span>
      </div>
      <div class="skill">
        <i class="fa-solid fa-database"></i>
        <span>Mysql</span>
      </div>
      <div class="skill">
        <i class="fa-brands fa-figma"></i>
        <span>Figma</span>
      </div>
    </div>
    <br /><br />

    <button class="btnCV">
      <a href="#" class="yes" target="_blank"> Download CV </a>
    </button>
    <br /><br />
    <h1>Soft Skills</h1>
    <div class="soft-skills">
      <div class="skill">
        <i class="fa-solid fa-paintbrush"></i>
        <span>Creativity</span>
      </div>
      <div class="skill">
        <i class="fa-solid fa-business-time"></i>
        <span>Time Management</span>
      </div>
      <div class="skill">
        <i class="fa-solid fa-people-arrows"></i>
        <span>Communication</span>
      </div>
      <div class="skill">
        <i class="fa-solid fa-infinity"></i>
        <span>Adaptability</span>
      </div>
    </div>
    <h1>My Education:</h1>
    <div class="container">
      <div class="card">
        <div class="content">
          <h2>2009 - 2015</h2>
          <p>I attended Turfhall Primary School and graduated in 2015.</p>
          <a href="#">Turfhall Primary School</a>
        </div>
        <img
          src="https://i.postimg.cc/zVGVcGgp/Screenshot-2023-11-01-110851-removebg-preview.png[/img][/url]
  "
          alt=""
        />
      </div>
      <div class="card">
        <div class="content">
          <h2>2016 - 2020</h2>
          <p>
            I attended Windsor High School and graduated Matic with a bachelors
            Pass .
          </p>
          <a href="#">Windsor High School</a>
        </div>
        <img
          src="https://i.postimg.cc/0rx67f5T/Screenshot-2023-11-01-110948-removebg-preview.png[/img][/url]
  "
          alt=""
        />
      </div>
      <div class="card">
        <div class="content">
          <h2>2023 - Present</h2>
          <p>
            I am currently studing a Coding Course at Life Choices Academy,
            seeking a career in website development.
          </p>
          <a href="#">Life Choices Academy</a>
        </div>
        <img
          src="https://i.postimg.cc/tJJvp3HH/1000025647-removebg-preview-1.png"
          alt=""
        />
      </div>
    </div>
    <h1>My Job Experience:</h1>
    <div class="container">
      <div class="card1">
        <div class="content">
          <h2>Jan - Dec 2021</h2>
          <p>
            I'd done some volunteer work for my community during the year of
            2021 offering assistence with what ever was needed like clean up
            work or organizing functions for the community. As this was
            technically my first job i learnt was the work place was like an
            what i would need to prepare for.
          </p>
          <a href="#">Volunteer Work</a>
        </div>
      </div>
      <div class="card1">
        <div class="content">
          <h2>Jan - Dec 2022</h2>
          <p>
            During the year of 2022 for a temporary period was handling a small
            fishing entrepreneur handle their employees payroll while he was
            under staffed. While doing this i was gaining a lot of experience in
            the finance field.
          </p>
          <a href="#">Payroll Administrator</a>
        </div>
      </div>
      <div class="card1">
        <div class="content">
          <h2>Jan - Mar 2023</h2>
          <p>
            I took the decision to help out the people in my area with transport
            since i had gotten my license so i started to drop off an pick up
            the elderly people in my community when it was their pension which
            was a small income for me and was better for them then taking public
            transport.
          </p>
          <a href="#">Community transport driver</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script></script>

<style scoped>
#resume {
  width: 100vw;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.container {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  /* background-image: url(https://i.postimg.cc/HsBNKSnJ/Screenshot-2024-01-08-144001.png); */
}
.skills-container1,
.skills-container2,
.soft-skills {
  font-size: 130px;
  color: gold;
  gap: 30px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.skill .fa-html5,
.fa-css3-alt,
.fa-bootstrap,
.fa-js,
.fa-vuejs,
.fa-database,
.fa-figma {
  transition: 0.5s ease all;
}
.skill .fa-html5:hover {
  transform: scale(1.2);
  color: tomato;
}
.skill .fa-css3-alt:hover {
  transform: scale(1.2);
  color: teal;
}
.skill .fa-bootstrap:hover {
  transform: scale(1.2);
  color: purple;
}
.skill .fa-js:hover {
  transform: scale(1.2);
  color: yellow;
}
.skill .fa-vuejs:hover {
  transform: scale(1.2);
  color: forestgreen;
}
.skill .fa-database:hover {
  transform: scale(1.2);
  color: aquamarine;
}
.skill .fa-figma:hover {
  transform: scale(1.2);
  color: rebeccapurple;
}

.skills-container1 {
  justify-content: space-evenly;
}

.skills-container2 {
  justify-content: space-evenly;
}

.skill {
  text-align: center;
}

.skill span {
  font-size: 14px;
  display: block;
}

.container .card {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 320px;
  margin: 40px;
  background: #222;
  border: 2px solid gold;
  border-radius: 40px;
  transition: 0.5s ease;
  transition: 2.5s ease;
}
.container .card1 {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 320px;
  /* margin: 40px; */
  margin-bottom: 20px;
  background: #444;
  border: 3px solid gold;
  border-radius: 40px;
  transition: 0.5s ease;
  transition: 2.5s ease;
}

.container .card:hover {
  box-shadow: 0 0px 20px gold;
  border: 3px solid black;
}
.container .card1:hover {
  box-shadow: 0 0px 20px gold;
  border: 3px solid black;
}

.container .card1:hover {
  background: gold;
}

.container .card:nth-child(1):hover {
  background: gold;
}

.container .card:nth-child(2):hover {
  background: gold;
}

.container .card:nth-child(3):hover {
  background: gold;
}

.container .card img {
  position: absolute;
  height: 200px;
  width: 200px;
  transition: 3s ease;
}

.container .card:nth-child(1) img {
  height: 230px;
  width: fit-content;
  transition: 1s;
}

.container .card:nth-child(2) img {
  height: 230px;
  width: fit-content;
  transition: 1s;
}

.container .card:nth-child(3) img {
  height: 230px;
  width: fit-content;
  transition: 1s;
}

.container .card:nth-child(1):hover img {
  opacity: 0; /* Setting opacity to 0 when hovered over */
}

.container .card:nth-child(2):hover img {
  opacity: 0; /* Setting opacity to 0 when hovered over */
}

.container .card:nth-child(3):hover img {
  opacity: 0; /* Setting opacity to 0 when hovered over */
}

.container .card:nth-child(1) .content,
.container .card:nth-child(2) .content,
.container .card:nth-child(3) .content {
  position: relative;
  width: 350px;
  opacity: 0;
  visibility: hidden;
  transition: 1s ease;
}

.container .card1 .content {
  position: relative;
  width: 350px;
  transition: 1s ease;
}

.container .card:hover .content {
  left: 0;
  visibility: visible;
  opacity: 1;
}

.content h2 {
  font-family: "Permanent Marker", cursive;
  color: #111;
  text-transform: uppercase;
  text-shadow: 1px 1px 0.1em rgba(0, 0, 0, 0.3);
  font-size: 2.2em;
  line-height: 1em;
}

.content p {
  font-family: "Roboto", sans-serif;
  font-weight: bold;
  color: #111;
  margin: 20px 0 20px;
}

.content a {
  font-family: "Roboto", sans-serif;
  position: relative;
  color: #555;
  background: #fafafa;
  border-radius: 2px;
  box-shadow: 1px 1px 0.2em rgba(0, 0, 0, 0.3);
  padding: 5px 20px;
  text-decoration: none;
  font-weight: 500;
}

/* Responsive styles */
@media only screen and (max-width: 780px) {
  .container {
    flex-direction: column;
    align-items: center;
  }

  .card,
  .card1 {
    width: 100%;
  }
}
</style>
