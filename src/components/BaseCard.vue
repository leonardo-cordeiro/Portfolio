<template>
  <div class="project-card">
    <a :href="link" target="_blank" class="project-link">
      <div class="project-image">
        <img :src="img" :alt="title" class="project-img" />
      </div>
    </a>
    <div class="project-details">
      <h3 class="project-title">{{ title }}</h3>
      <p class="project-description">{{ description }}</p>
      <div class="project-languages">
        <div class="language">
          <img v-if="html" src="@/assets/img/html.svg" alt="HTML" />
        </div>
        <div class="language">
          <img v-if="vue" src="src/icons/icons8-vue-js.svg" alt="Vue.js" />
        </div>
        <div class="language">
          <img v-if="css" src="@/assets/img/css-3-svgrepo-com.svg" alt="CSS" />
        </div>
        <div class="language">
          <img v-if="javascript" src="src/icons/icons8-javascript-240.png" alt="JavaScript" />
        </div>
      </div>
    </div>
    <!-- <a :href="github" class="github-link">
      <img src="src/icons/icons8-github.svg" alt="GitHub" />
    </a> -->
  </div>
</template>

<script setup>
defineProps({
  title: String,
  description: String,
  img: String,
  html: Boolean,
  css: Boolean,
  javascript: Boolean,
  vue: Boolean,
  link: String,
  github: String
})
</script>

<style scoped>
.project-card {
  margin: 15px;
  border: 2px solid #fff;
  border-radius: 5%;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  width: calc(33% - 30px);
  height: 100%;
}

.project-image {
  overflow: hidden;
}

.project-img {
  width: 100%;
  height: 100%;
  /* border-radius: 10px; */
  cursor: pointer;
}

.project-details {
  padding: 10px;
  background-color: rgba(241, 241, 241, 0.541);
  display: flex;
  flex-direction: column;
  /* align-items: center; */
  /* justify-content: center; */
  /* text-align: center; */
  color: #000;
  text-decoration: none;
}

.project-title {
  font-size: 1.5rem;
  margin-bottom: 5px;
}

.project-description {
  font-size: 1rem;
}

.project-languages {
  display: flex;
  /* justify-content: space-between; */
  align-items: center;
  margin-top: 10px;
}

.language {
  width: 30px;
  height: 100%;
}

.language img {
  width: 100%;
  height: 100%;
}

.github-link {
  margin-top: auto;
  text-align: right;
  padding: 10px;
}
</style>
