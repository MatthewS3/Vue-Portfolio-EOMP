<template>
  <div id="home">
    <div class="box7"></div>
    <div class="fade-in-text">
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
      </div>
      <div class="text">ASPIRING</div>
      <div class="text">
        <span>Web & Software Developer</span>
      </div>
      <section>
        <div class="ease-in">
          <p class="ease-in">
            I have a trumendous passion for Web designing as well as interactive, and
            responsive websites and i am fulfilling a dream of mine to become a Web
            Developer.
          </p>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeView",
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&display=swap');

#home {
  height: 610px;
  background-image: url(https://i.postimg.cc/HsBNKSnJ/Screenshot-2024-01-08-144001.png);
  display: flex;
  justify-content: center;
  padding: 65px;
}

.name {
  color: gold;
}

.fade-in-text {
  width: 600px;
  text-align: center;
  font-family: "Playfair Display", serif;
  animation: fadeIn 5s;
}

.waviy {
  position: relative;
  font-size: 60px;
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

.box7 {
  height: 400px;
  width: 400px;
  border: 5px transparent;
  border-radius: 20px;
  margin-left: -100px;
  box-shadow: rgba(0, 0, 0, 0.3);
  background-image: url(https://i.postimg.cc/DzpBrj7M/1000025647-removebg-preview-2.png);
  animation-delay: 5s;
  animation: fadeIn 8s;
}

.btn {
  background-color: gold;
  font-size: 20px;
  font-family: "Playfair Display", serif;
  height: 40px;
  width: 130px;
  border-radius: 100px;
  cursor: pointer;
}

.btn:hover {
  background-color: black;
  color: gold;
  transition: 2.5s;
}
.ease-in {
  font-size: 25px;
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
  display:inline-block;
  overflow:hidden;
  color: gold;
  font-size: 28px;
}

.text:first-of-type { 
  animation: showup 7s infinite;
}

.text:last-of-type {
  width:0px;
  animation: reveal 7s infinite;
}

.text:last-of-type span {
  margin-left:-355px;
  animation: slidein 7s infinite;
}

@keyframes showup {
    0% {opacity:0;}
    20% {opacity:1;}
    80% {opacity:1;}
    100% {opacity:0;}
}

@keyframes slidein {
    0% { margin-left:-800px; }
    20% { margin-left:-800px; }
    35% { margin-left:0px; }
    100% { margin-left:0px; }
}

@keyframes reveal {
    0% {opacity:0;width:0px;}
    20% {opacity:1;width:0px;}
    30% {width:355px;}
    80% {opacity:1;}
    100% {opacity:0;width:355px;}
}


p {
  font-size:12px;
  color:#999;
  margin-top:100px;

}
</style>
