<template>
  <div id="Projects">
    <h1>My Projects</h1>
    <section class="wwww">
      <div class="container">
        <div class="row mt-5">
          <div class="col">
            <div class="card-container" id="demo">
              <div class="cardww" tabindex="0">
                <h2>
                  JS E-Commerce
                  <br />
                  Website:
                </h2>
                <img
                  src="https://i.postimg.cc/d1XycDkN/Screenshot-2024-01-12-083000.png"
                  width="100%"
                />
                  <a href="https://takealittle-ecommerce-website.netlify.app/"
                    ><button class="btn">
                      <span>Host Link</span>
                    </button></a
                  >
                  <a href="https://github.com/MatthewS3/E-Commerce-JS-EOMP"
                    ><button class="btn">
                      <span>GitHub</span>
                    </button></a
                  >
              </div>
              <div class="cardww" tabindex="0">
                <h2>
                  Hex To Rgb
                  <br />
                  Converter:
                </h2>
                <img
                  src="https://i.postimg.cc/Gmf9XK90/Screenshot-2024-01-12-093130.png"
                  width="100%"
                />
                <a href="https://hex-rgb-converter.netlify.app/"
                  ><button class="btn">
                    <span>Host Link</span>
                  </button></a
                >
                <a href="https://github.com/MatthewS3/HexToRGB"
                  ><button class="btn">
                    <span>GitHub</span>
                  </button></a
                >
              </div>
              <div class="cardww" tabindex="0">
                <h2>
                  Rgb to Hex
                  <br />
                  Converter:
                </h2>
                <img
                  src="https://i.postimg.cc/0jZ7jSn8/Screenshot-2024-01-12-093325.png"
                  width="100%"
                />
                <a href="https://rgb-to-hex-converter1.netlify.app/"
                  ><button class="btn">
                    <span>Host Link</span>
                  </button></a
                >
                <a href="https://github.com/MatthewS3/RGBtoHEX"
                  ><button class="btn">
                    <span>GitHub</span>
                  </button></a
                >
              </div>
              <div class="cardww" tabindex="0">
                <h2>Js <br> Calculator:</h2>
                <img
                  src="https://i.postimg.cc/90qr5qk8/Screenshot-2024-01-12-093532.png"
                  width="100%"
                />
                <a href="https://javascript-calculator-ms.netlify.app/"
                  ><button class="btn">
                    <span>Host Link</span>
                  </button></a
                >
                <a href="https://github.com/MatthewS3/JavaScript_Calc"
                  ><button class="btn">
                    <span>GitHub</span>
                  </button></a
                >
              </div>
              <div class="cardww" tabindex="0">
                <h2>Interest Rate <br> Calculator:</h2>
                <img
                  src="https://i.postimg.cc/wMqYVZmQ/Screenshot-2024-01-12-094645.png"
                  width="100%"
                />
                <a href="https://interest-rate-calculatortor.netlify.app/"
                  ><button class="btn">
                    <span>Host Link</span>
                  </button></a
                >
                <a href="https://github.com/MatthewS3/Interest-Calculator"
                  ><button class="btn">
                    <span>GitHub</span>
                  </button></a
                >
              </div>
              <div class="cardww" tabindex="0">
                <h2>YouTube <br> Cloned Website:</h2>
                <img
                  src="https://i.postimg.cc/vTtYrLxV/Screenshot-2024-01-12-094317.png"
                  width="100%"
                />
                <a href="https://youtube-clone-web-ms.netlify.app/"
                  ><button class="btn">
                    <span>Host Link</span>
                  </button></a
                >
                <a href="https://github.com/MatthewS3/YouTube_Clone"
                  ><button class="btn">
                    <span>GitHub</span>
                  </button></a
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script></script>

<style scoped>
.card-container {
  display: flex;
  padding: 2rem 2rem;
  width: auto;
}

.cardww {
  flex: 1;
  transition: all 0.4s ease-in-out;
  background-color: #333;
  color: gold;
  padding: 10px;
  border-radius: 40px;
  border: solid 4px black;
}
.cardww h2 {
  font-size: 22px;
}
.cardww:not(:first-child) {
  margin-left: -7rem;
}
 img {
  padding: 35px;
  width: 200px;
  height: 150px;
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

@media (max-width: 780px) {
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
  font-size: 15px;
  background-color: #111;
  padding: 10px 20px;
  margin: 0 auto;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 20.2);
  -webkit-transition: all 0.5s ease-in-out;
  transition: all 0.5s ease-in-out;
  border-radius: 50px;
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
}

@media (max-width: 780px) {
  .card-container {
    display: grid;
    padding: 0rem 0rem;
    flex-direction: column;
    width: auto;
  }
  .cardww {
    flex: 1;
    transition: all 0.4s ease-in-out;
    background-color: #333;
    color: gold;
    padding: 10px;
    border-radius: 40px;
    border: solid 4px black;
  }
  .cardww h2 {
    font-size: 10px;
  }
}
</style>
