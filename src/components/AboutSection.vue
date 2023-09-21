<template>
  <div class="wrap">
    <div class="title">
      <h1>About me</h1>
    </div>

    <div class="text">
      <p>
        I'm Leonardo Gama, a dedicated Front-End developer skilled in Vue.js. My journey in
        technology is driven by determination, unwavering focus, and a knack for effective teamwork.
        With experience honed during almost three years in the United States, I've attained an
        advanced level of English proficiency. I excel in crafting impactful digital experiences
        that leave a lasting mark. Beyond coding, my commitment to collaboration and my global
        perspective enable me to engage with diverse stakeholders effectively. I'm an enthusiastic
        problem solver always seeking fresh challenges and innovative projects. I'm ready to
        contribute my expertise and passion to the ever-evolving field of Front-End development.
      </p>
      <img src="src/img/foto_about.jpg" alt="" />
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.wrap {
  position: relative;
  display: block;
  background: #ffffff;
}
/* 
.title {
  text-align: center;
} */

.text {
  display: flex;
  text-align: start;
  letter-spacing: 2.5px;
  padding: 10px;
  margin-right: 50px;
}

.text img {
  width: 40%;
  margin-left: 30px;
  border-radius: 20% 0 20% 0;
}
</style>
