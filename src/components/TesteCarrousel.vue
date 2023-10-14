<template>
  <div class="slider">
    <div class="slide-track">
      <div class="slide">
        <img src="../assets/icons/icons8-html-5-240.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/css-3.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/icons8-javascript-240.png" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/icons8-vue-js.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/icons8-bootstrap.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/icons8-firebase.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/icons8-git.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/tailwindcss-icon.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/python-icon.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/icons8-mysql-logo.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/icons8-firebase.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/icons8-git.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="../assets/icons/tailwindcss-icon.svg" height="100" width="100" alt="" />
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
@-webkit-keyframes scroll {
  0% {
    -webkit-transform: translateX(0);
    transform: translateX(0);
  }
  100% {
    -webkit-transform: translateX(calc(-250px * 7));
    transform: translateX(calc(-250px * 7));
  }
}
@keyframes scroll {
  0% {
    -webkit-transform: translateX(0);
    transform: translateX(0);
  }
  100% {
    -webkit-transform: translateX(calc(-250px * 7));
    transform: translateX(calc(-250px * 7));
  }
}
.slider {
  background: pr;
  box-shadow: 0 10px 20px -5px rgba(0, 0, 0, 0.125);
  margin: auto;
  overflow: hidden;
  position: relative;
  width: 100%;
  background-color: #1f0287;
}
.slider::before,
.slider::after {
  content: '';
  height: 100px;
  position: absolute;
  width: 200px;
  z-index: 2;
}
.slider::after {
  right: 0;
  top: 0;
  -webkit-transform: rotateZ(180deg);
  transform: rotateZ(180deg);
}
.slider::before {
  left: 0;
  top: 0;
}
.slider .slide-track {
  -webkit-animation: scroll 10s linear infinite;
  animation: scroll 10s linear infinite;
  display: flex;
  width: calc(250px * 14);
}
.slider .slide {
  height: 100px;
  width: 250px;
}

.slide img {
  height: 60px;
  width: 60px;
  margin-top: 20px;
}
</style>
