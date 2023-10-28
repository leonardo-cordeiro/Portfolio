<template>
  <!-- <p>Hello World</p> -->
  <div class="slider">
    <div class="slide-track" :style="{ transform: `translateX(${offset}px)` }">
      <h2 class="slider-title">Skills:</h2>
      <div class="slide">
        <img src="/icons/icons8-html-5-240.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="/icons/css-3.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="/icons/icons8-javascript-240.png" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="/icons/icons8-vue-js.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="/icons/icons8-bootstrap.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="/icons/icons8-firebase.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="/icons/icons8-git.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="/icons/icons8-mysql-logo.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="/icons/tailwindcss-icon.svg" height="100" width="100" alt="" />
      </div>
      <div class="slide">
        <img src="/icons/python-icon.svg" height="100" width="100" alt="" />
      </div>
    </div>
    <button class="prev" @click="slide('prev')">&#10094;</button>
    <button class="next" @click="slide('next')">&#10095;</button>
  </div>
</template>
<!-- 
<template>
  <div style="width: 100vw">
    <div class="teste"></div>
  </div>
  <Splide extensions="" :options="config" aria-label="My Favorite Images">
    <SplideSlide>
      <img src="image1.jpg" alt="Sample 1" />
    </SplideSlide>
    <SplideSlide>
      <img src="image2.jpg" alt="Sample 2" />
    </SplideSlide>
    <SplideSlide>
      <img src="image2.jpg" alt="Sample 2" />
    </SplideSlide>
    <SplideSlide>
      <img src="image2.jpg" alt="Sample 2" />
    </SplideSlide>
    <SplideSlide>
      <img src="image2.jpg" alt="Sample 2" />
    </SplideSlide>
    <SplideSlide>
      <img src="image2.jpg" alt="Sample 2" />
    </SplideSlide>
  </Splide>
</template> -->

<script setup>
// import { Splide, SplideSlide } from '@splidejs/vue-splide'
// import { AutoScroll } from '@splidejs/splide-extension-auto-scroll'
// import '@splidejs/vue-splide/css'

// const config = {
//   rewind: true,
//   drag: false,
//   autoScroll: {
//     speed: 1
//   },
//   autoplay: true
// }
import { ref } from 'vue'

const offset = ref(0)
const slideWidth = 460
const totalSlides = 10.5

const slide = (direction) => {
  const maxOffset = -(slideWidth * (totalSlides - 9))

  if (direction === 'prev') {
    offset.value = Math.min(offset.value + slideWidth, 0)
  } else if (direction === 'next') {
    offset.value = Math.max(offset.value - slideWidth, maxOffset)
  }
}
</script>

<style scoped>
.teste {
  background-color: #1766aa;
  margin: 20px;
  border: 5px solid #333;
  width: 150px;
  height: 150px;
  border-radius: 50%;
  animation: 3s linear 1s infinite running slidein;
}

.slider {
  background: pr;
  box-shadow: 0 10px 20px -5px rgba(0, 0, 0, 0.125);
  margin: auto;
  overflow: hidden;
  position: relative;
  width: 100%;
  /* background-color: #1f0287; */
  background-color: #cedfdf;
  display: flex;
}

.slide-track {
  display: flex;
  transition: transform 0.5s ease;
}

.slide {
  height: 100px;
  width: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.slider-title {
  color: #fff;
  font-size: 2rem;
  text-align: center;
  margin-left: 4rem;
  margin-top: 2.5rem;
}

.slide img {
  height: 60px;
  width: 60px;
  margin-top: 20px;
}

.prev,
.next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background-color: rgba(0, 0, 0, 0.5);
  color: #fff;
  cursor: pointer;
  padding: 10px;
  border: none;
  z-index: 3;
}

.prev {
  left: 0;
}

.next {
  right: 0;
}
</style>
