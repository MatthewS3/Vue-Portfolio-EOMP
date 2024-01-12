<template>
  <h1>My Skills:</h1>
  <section>
  <div class="skills">
    <div class="skills-bar">
      <div class="bar">
        <div class="info">
          <span>HTML</span>
        </div>
        <div class="progress-line"><span class="html"></span></div>
        <div class="bar">
          <div class="info">
            <span>CSS</span>
          </div>
          <div class="progress-line"><span class="css"></span></div>
          <div class="bar">
            <div class="info">
              <span>BOOTSTRAP</span>
            </div>
            <div class="progress-line"><span class="bootstrap"></span></div>
            <div class="bar">
              <div class="info">
                <span>JAVASCRIPT</span>
              </div>
              <div class="progress-line">
                <span class="javascript"></span>
              </div>
              <div class="bar">
                <div class="info">
                  <span>Vue.JS</span>
                </div>
                <div class="progress-line"><span class="c"></span></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  </section>
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
        <p>I attended Windsor High School and graduated Matic with a bachelors Pass .</p>
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
          I am currently studing a Coding Course at Life Choices Academy, seeking a career
          in website development.
        </p>
        <a href="#">Life Choices Academy</a>
      </div>
      <img src="https://i.postimg.cc/tJJvp3HH/1000025647-removebg-preview-1.png" alt="" />
    </div>
  </div>
  <h1>My Job Experience:</h1>
  <div class="container">
    <div class="card">
      <div class="content">
        <h2>Jan - Dec 2021</h2>
        <p>
          I'd done some volunteer work for my community during the year of 2021 offering
          assistence with what ever was needed like clean up work or organizing functions
          for the community. As this was technically my first job i learnt was the work
          place was like an what i would need to prepare for.
        </p>
        <a href="#">Volunteer Work</a>
      </div>
      <img src="" alt="" />
    </div>
    <div class="card">
      <div class="content">
        <h2>Jan - Dec 2022</h2>
        <p>
          During the year of 2022 for a temperary period was handling a small fishing
          entrepreneur handle their employees payroll while he was under staffed. While
          doing this i was gaining alot of experience in the finance field.
        </p>
        <a href="#">Payroll Administrator</a>
      </div>
      <img
        src=""
        alt=""
      />
    </div>
    <div class="card">
      <div class="content">
        <h2>Jan - Mar 2023</h2>
        <p>
          I took the decision to help out the people in my area with transport since i had
          gotten my license so i started to drop off an pick up the elderly people in my
          community when it was their pension which was a small income for me and was
          better for them then taking public transport.
        </p>
        <a href="#">Community transport driver</a>
      </div>
      <img
        src=""
        alt=""
      />
    </div>
  </div>
</template>

<script></script>

<style>
.skills {
  position: relative;
  width: 470px;
  top: 200px;
  left: 50%;
  transform: translate(-50%, -50%);
  background: #222;
  border-radius: 50px;
  box-shadow: 0 19px 38px rgba(0, 0, 0, 0.3), 0 15px 12px rgba(0, 0, 0, 0.22);
}

.skills-bar {
  padding: 25px 30px;
}

.skills-bar .bar {
  margin: 25px 0;
}

.skills-bar .bar .info span {
  font-size: 1rem;
  font-weight: 500;
}

.skills-bar .bar .info {
  margin-bottom: 8px;
  color: gold;
}

.skills-bar .bar .progress-line {
  position: relative;
  align-content: center;
  height: 10px;
  width: 450px;
  margin-left: -245px;
  background: transparent;
  border-radius: 10px;
  transform: scaleX(0);
  transform-origin: center;
  animation: animate 5s cubic-bezier(1, 0, 0.5, 1) forwards;
}

.bar .progress-line span {
  position: absolute;
  background: gold;
  height: 100%;
  border-radius: 10px;
  transform: scaleX(0px);
  transform-origin: center;
  animation: animate 5s 1s cubic-bezier(1, 0, 0.5, 1) forwards;
}

@keyframes animate {
  100% {
    transform: scaleX(1);
  }
}

.progress-line .html {
  width: 75%;
}
.progress-line .css {
  width: 70%;
}
.progress-line .bootstrap {
  width: 68%;
}
.progress-line .javascript {
  width: 40%;
}
.progress-line .c {
  width: 30%;
}

.bar .progress-line span::before {
  position: absolute;
  content: "";
  height: 0;
  right: 0;
  top: -14px;
  width: 0;
  border: 7px solid transparent;
  border-bottom-width: 0px;
  border-right-width: 0px;
  border-top-style: #f0f0f0;
  border-top-color: #111;
}

.bar .progress-line span::after {
  position: absolute;
  right: 0;
  top: -28px;
  color: #f0f0f0;
  font-size: 12px;
  font-weight: 700;
  background: #111;
  padding: 1px 8px;
  border-radius: 3px;
}


.progress-line .html::after {
  content: "%";
}
.progress-line .css::after {
  content: "%";
}
.progress-line .bootstrap::after {
  content: "%";
}
.progress-line .javascript::after {
  content: "%";
}
.progress-line .c::after {
  content: "%";
}

/* ////........Media Query........//// */

@media (max-width: 700px) {
    .skills{
        width: 80%;
    }

    .skills-bar .bar .progress-line{
        width: 100%;
    }
}


.container {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  /* background-image: url(https://i.postimg.cc/HsBNKSnJ/Screenshot-2024-01-08-144001.png); */
}

.container .card {
  position: relative;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  width: 400px;
  height: 320px;
  margin: 40px;
  background: #222;
  border-top: 1px solid rgba(255, 255, 255, 0.4);
  border-left: 1px solid rgba(255, 255, 255, 0.4);
  backdrop-filter: blur(5px);
  box-shadow: -5px 5px 0.4em rgba(0, 0, 0, 0.1);
  border-radius: 4px;
  transition: 0.5s ease;
}

.container .card:hover {
  transition: 2.5s ease;
  margin-right: 10px;
  width: 450px;
}

.container .card:nth-child(1):hover {
  background: rgba(246, 188, 15, 0.7);
}

.container .card:nth-child(2):hover {
  background: rgba(246, 188, 15, 0.7);
}

.container .card:nth-child(3):hover {
  background: rgba(246, 188, 15, 0.7);
}

.container .card img {
  position: absolute;
  left: 20%;
  transform: translateX(0%);
  height: 300px;
  transition: 3s ease;
}

.container .card:nth-child(1) img {
  height: 230px;
}

.container .card:hover img {
  left: 75%;
  height: 100px;
}

.container .card:nth-child(1):hover img {
  left: 65%;
  height: 100px;
}

.container .card:nth-child(3):hover img {
  left: 80%;
  height: 100px;
}

.container .card .content {
  position: relative;
  width: 300px;
  left: 20%;
  opacity: 0;
  visibility: hidden;
  padding: 20px 20px 20px 40px;
  transition: 2.5s ease;
}

.container .card:hover .content {
  left: 0;
  visibility: visible;
  opacity: 1;
}

.content h2 {
  font-family: "Permanent Marker", cursive;
  color: #fefefe;
  text-transform: uppercase;
  text-shadow: 1px 1px 0.1em rgba(0, 0, 0, 0.3);
  font-size: 2.2em;
  line-height: 1em;
}

.content p {
  font-family: "Roboto", sans-serif;
  color: #fefefe;
  margin: 20px 0 20px;
  font-weight: 400;
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
</style>
