<template>
  <br />
  <br />
  <br>
  <div id="Home">
    <div class="fade-in-text">
      <!-- <img
        src="https://i.postimg.cc/DzpBrj7M/1000025647-removebg-preview-2.png"
        alt="imageME"
      /> -->
      <div class="waviy">
        <span style="--i: 1">M</span>
        <span style="--i: 2">a</span>
        <span style="--i: 3">t</span>
        <span style="--i: 4">t</span>
        <span style="--i: 5">h</span>
        <span style="--i: 6">e</span>
        <span style="--i: 7">w</span>
        <br />
        <span style="--i: 8">S</span>
        <span style="--i: 9">w</span>
        <span style="--i: 11">a</span>
        <span style="--i: 12">i</span>
        <span style="--i: 13">n</span>
        <span style="--i: 14">'</span>
        <span style="--i: 15">s</span>
        <br />
        <span style="--i: 16">P</span>
        <span style="--i: 17">o</span>
        <span style="--i: 18">r</span>
        <span style="--i: 19">t</span>
        <span style="--i: 20">f</span>
        <span style="--i: 21">o</span>
        <span style="--i: 22">l</span>
        <span style="--i: 23">i</span>
        <span style="--i: 24">o</span>
        <div class="ease-in">
          <div class="text">ASPIRING</div>
          <div class="text">
            <span>Web & Software Developer</span>
          </div>
        </div>
        <p class="ease-in">
          "I have a tremendous passion for Web designing as well as
          interactive, and responsive websites and i am fulfilling a dream of
          mine to become a Developer"
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeView",
};
</script>

<style scoped>

.fade-in-text {
  justify-content: center;
  font-family: "Playfair Display", serif;
  animation: fadeIn 5s;
  display: flex;
}

.waviy {
  position: relative;
  width: 700px;
  font-size: 60px;
  /* margin-left: 50px; */
}
.waviy span {
  font-family: "Playfair Display", serif;
  position: relative;
  display: inline-block;
  color: gold;
  text-transform: uppercase;
  animation: waviy 3s infinite;
  animation-delay: calc(0.1s * var(--i));
}

@keyframes waviy {
  0%,
  60%,
  100% {
    transform: translateY(0);
  }
  20% {
    transform: translateY(-15px);
  }
}

.ease-in {
  font-size: 25px;
  font-weight: bold;
  margin-bottom: 20px;
  animation: color-change 10s infinite;
}

@keyframes color-change {
  0% {
    color: white;
  }
  25% {
    color: goldenrod;
  }
  50% {
    color: gold;
  }
  75% {
    color: goldenrod;
  }
  100% {
    color: white;
  }
}

.text {
  display: inline-block;
  overflow: hidden;
  color: gold;
  font-size: 20px;
}

.text:first-of-type {
  animation: showup 7s infinite;
}

.text:last-of-type {
  width: 0px;
  animation: reveal 7s infinite;
}

.text:last-of-type span {
  margin-left: -355px;
  animation: slidein 7s infinite;
}

@keyframes showup {
  0% {
    opacity: 0;
  }
  20% {
    opacity: 1;
  }
  80% {
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}

@keyframes slidein {
  0% {
    margin-left: -800px;
  }
  20% {
    margin-left: -800px;
  }
  35% {
    margin-left: 0px;
  }
  100% {
    margin-left: 0px;
  }
}

@keyframes reveal {
  0% {
    opacity: 0;
    width: 0px;
  }
  20% {
    opacity: 1;
    width: 0px;
  }
  30% {
    width: 355px;
  }
  80% {
    opacity: 1;
  }
  100% {
    opacity: 0;
    width: 355px;
  }
}

p {
  font-size: 12px;
  color: #999;
  margin-top: 100px;
}

/* <<=======MEDIA QUERIES======>> */

@keyframes wave-animation {
  0% {
    transform: translateY(0);
  }
  100% {
    transform: translateY(-10px);
  }
}

@keyframes fadeIn {
  0% {
    opacity: 0;
    transform: scale(0.8);
  }
  100% {
    opacity: 1;
    transform: scale(1);
  }
}

@media (max-width: 780px){
  .text:last-of-type {
  width: 100px;
  animation: reveal 7s 1;
  height: 100px !important;
  overflow: hidden
}

.ease-in {
  font-size: 15px;
  font-weight: bold;
  margin-bottom: 20px;
  animation: color-change 10s 1;
}

@keyframes reveal {
  0% {
    opacity: 0;
    width: 0px;
  }
  20% {
    opacity: 1;
    width: 0px;
  }
  30% {
    width: 255px;
  }
  80% {
    opacity: 1;
  }
  100% {
    opacity: 0;
    width: 255px;
  }
}

}

/* Responsive styles */
@media only screen and (max-width: 600px) {
      .fade-in-text {
        padding: 0px;
      }

      .waviy {
        width: 100%; /* Adjust the width */
      }
    }
</style>
