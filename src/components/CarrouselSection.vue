<template>
  <section id="slideshow">
    <div class="entire-content">
      <div class="content-carrousel">
        <figure class="shadow">
          <img src="src/icons/icons8-javascript-240.png" alt="Alan Walker - The Spectre" />
        </figure>
        <figure class="shadow">
          <img src="src/icons/icons8-html-5-240.svg" alt="Alan Walker - Alone" />
        </figure>
        <figure class="shadow">
          <img src="src/icons/icons8-bootstrap.svg" alt="OM TELOLET OM - ALAN WALKER" />
        </figure>

        <figure class="shadow">
          <img src="src/icons/icons8-vue-js.svg" alt="Alan Walker - The Spectre" />
        </figure>
        <figure class="shadow">
          <img
            src="src/icons/icons8-mysql-logo.svg"
            alt="Alan Walker has partnered with Battlefield to showcase his new track Alone"
          />
        </figure>
        <figure class="shadow">
          <img
            src="src/icons/tailwindcss-icon.svg"
            alt="The Drop Dancing GIF by Alan Walker Official"
          />
        </figure>
        <figure class="shadow">
          <img src="src/icons/w3_css-icon.svg" alt="alone GIF by Alan Walker Official" />
        </figure>
        <figure class="shadow">
          <img src="src/icons/icons8-git.svg" alt="alone GIF by Alan Walker Official" />
        </figure>
        <figure class="shadow">
          <img src="src/icons/python-icon.svg" alt="sing me to sleep GIF by Alan Walker Official" />
        </figure>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
#slideshow {
  width: 100%;
  background-repeat: no-repeat;
  background-size: cover;
}
.entire-content {
  margin-top: 50px;
  margin-left: 932px;
  width: 50px;
  perspective: 100%;
  position: relative;
}

.content-carrousel {
  width: 100%;
  position: absolute;
  float: right;
  animation: rotar 15s infinite linear;
  transform-style: preserve-3d;
}

.content-carrousel:hover {
  animation-play-state: paused;
  cursor: pointer;
}

.content-carrousel figure {
  width: 100%;
  height: 50px;
  overflow: hidden;
  /* position: absolute; */
}

.content-carrousel figure:nth-child(1) {
  transform: rotateY(0deg) translateZ(300px);
}
.content-carrousel figure:nth-child(2) {
  transform: rotateY(40deg) translateZ(300px);
}
.content-carrousel figure:nth-child(3) {
  transform: rotateY(80deg) translateZ(300px);
}
.content-carrousel figure:nth-child(4) {
  transform: rotateY(120deg) translateZ(300px);
}
.content-carrousel figure:nth-child(5) {
  transform: rotateY(160deg) translateZ(300px);
}
.content-carrousel figure:nth-child(6) {
  transform: rotateY(200deg) translateZ(300px);
}
.content-carrousel figure:nth-child(7) {
  transform: rotateY(240deg) translateZ(300px);
}
.content-carrousel figure:nth-child(8) {
  transform: rotateY(280deg) translateZ(300px);
}
.content-carrousel figure:nth-child(9) {
  transform: rotateY(320deg) translateZ(300px);
}
.content-carrousel figure:nth-child(10) {
  transform: rotateY(360deg) translateZ(300px);
}

.shadow {
  position: absolute;
  box-shadow: 0px 0px 10px 0px #000;
  border-radius: 5%;
  background-color: white;
}

.content-carrousel img {
  image-rendering: auto;
  transition: all 300ms;
  width: 100%;
  height: 100%;
}

.content-carrousel img:hover {
  transform: scale(1.2);
  transition: all 300ms;
}

@keyframes rotar {
  from {
    transform: rotateY(0deg);
  }
  to {
    transform: rotateY(360deg);
  }
}
</style>
