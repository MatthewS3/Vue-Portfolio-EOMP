<template>
  <div class="project">
    <h1>My Projects:</h1>
  </div>
  <section class="wwww">
    <div class="container">
      <div class="row mt-5">
        <div class="col">
          <div class="card-container" id="demo">
            <div class="cardww" tabindex="0">
              <h2>JS E-Commerce 
              <br>
              Website:</h2>
              <img
                src="https://i.postimg.cc/d1XycDkN/Screenshot-2024-01-12-083000.png"
                width="100%"
              />
              <div class="button_container">
              <a href="https://takealittle-ecommerce-website.netlify.app/"><button class="btn">
                <span>link.</span></button></a>
              </div>
            </div>
            <div class="cardww" tabindex="0">
              <h2>Hex To Rgb
              <br>
              Converter:</h2>
              <img
                src="https://i.postimg.cc/Gmf9XK90/Screenshot-2024-01-12-093130.png"
                width="100%"
              />
              <a href="https://hex-rgb-converter.netlify.app/"><button class="btn">
                <span>Link</span></button></a>
            </div>
            <div class="cardww" tabindex="0">
              <h2>Rgb to Hex
              <br>
              Converter:</h2>
              <img
                src="https://i.postimg.cc/0jZ7jSn8/Screenshot-2024-01-12-093325.png"
                width="100%"
              />
              <a href="https://rgb-to-hex-converter1.netlify.app/"><button class="btn">
                <span>Link</span></button></a>
            </div>
            <div class="cardww" tabindex="0">
              <h2>Js Calculator:</h2>
              <img
                src="https://i.postimg.cc/90qr5qk8/Screenshot-2024-01-12-093532.png"
                width="100%"
              />
              <a href="https://javascript-calculator-ms.netlify.app/"><button class="btn">
                <span>Link</span></button></a>
            </div>
            <div class="cardww" tabindex="0">
              <h2>Interest Rate Calculator:</h2>
              <img
                src="https://i.postimg.cc/wMqYVZmQ/Screenshot-2024-01-12-094645.png"
                width="100%"
              />
              <a href="https://interest-rate-calculatortor.netlify.app/"><button class="btn">
                <span>Link</span></button></a>
            </div>
            <div class="cardww" tabindex="0">
              <h2>YouTube Cloned Website:</h2>
              <img
                src="https://i.postimg.cc/vTtYrLxV/Screenshot-2024-01-12-094317.png"
                width="100%"
              />
              <a href="https://youtube-clone-web-ms.netlify.app/"><button class="btn">
                <span>Link</span></button></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script></script>

<style>
.card-container {
  display: flex;
  padding: 2rem 1rem;
}
.card-container .cardww {
  flex: 1;
  transition: all 0.3s ease-in-out;
  background-color: #333;
  color: gold;
  padding: 15px;
  border-radius: 30px;
  border: solid 2px black;

}
.cardww h2 {
  font-size: 22px;
}
.card-container .cardww:not(:first-child) {
  margin-left: -6rem;
}
.cardww img {
  padding: 35px;
  width: 200px;
  display: block;
  margin: 0 auto;
}
.card-container .cardww:hover,
.card-container .cardww:focus {
  transform: translateY(3rem);
  outline: none;
  background-color: #111;
  box-shadow: 0 5px 50px gold;

}
.card-container .cardww:hover ~ .cardww,
.card-container .cardww:focus ~ .cardww {
  transform: translateX(2.5rem);
}

@media (max-width: 767px) {
  #demo {
    margin-top: 0px;
  }

  .card-container {
    flex-wrap: wrap;
    justify-content: center;
    padding: 0rem 1rem 2rem;
  }
  .card-container .cardww {
    flex: 1 1 100%;
    max-width: 200px;
  }
  .card-container .cardww:not(:first-child) {
    margin-left: 0rem;
    margin-top: 2rem;
  }
  .card-container .cardww:hover,
  .card-container .cardww:focus {
    transform: translateX(0rem);
  }
  .card-container .cardww:hover ~ .cardww,
  .card-container .cardww:focus ~ .cardww {
    transform: translateY(0rem);
  }
  .cardww img {
    padding: 5px;
  }
}


.button_container {
	position: relative;
  left: 0;
  right: 0;
  top: 10%;
}

.btn {
  border: none;
  display: block;
  text-align: center;
  cursor: pointer;
  text-transform: uppercase;
  outline: none;
  overflow: hidden;
  position: relative;
  color: gold;
  font-weight: 700;
  font-size: 15px;
  background-color: #222;
  padding: 10px 20px;
  margin: 0 auto;
  box-shadow: 0 5px 15px rgba(0,0,0,20.20);
}

.btn span {
  position: relative; 
  z-index: 0;
}


.btn:hover {
  content: "";
  position: relative;
  left: 0;
  top: 0;
  background: gold;
  color: black;
  -webkit-transition: all 1.5s ease-in-out;
  transition: all 1.5s ease-in-out;

}
</style>
