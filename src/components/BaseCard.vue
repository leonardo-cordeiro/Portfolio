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
        <LanguageIcon v-if="vue" icon="src/icons/icons8-vue-js.svg" alt="Vue Logo" />
        <LanguageIcon v-if="javascript" icon="src/icons/icons8-javascript-240.png" alt="Vue Logo" />
        <LanguageIcon v-if="html" icon="src/icons/icons8-html-5-240.svg" alt="Vue Logo" />
        <LanguageIcon v-if="css" icon="src/icons/w3_css-icon.svg" alt="Vue Logo" />
        <a :href="github" class="github-link language">
          <LanguageIcon icon="src/icons/icons8-github.svg" alt="Github icon" />
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
import LanguageIcon from './LanguageIcon.vue'

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
  height: auto;
}

.project-img {
  width: 100%;
  height: 100%;
  cursor: pointer;
}

.project-details {
  padding-left: 10px;
  background-color: rgba(241, 241, 241, 0.541);
  display: flex;
  flex-direction: column;
  color: #000;
}

.project-title {
  font-size: 1.5rem;
  margin-bottom: 0px;
}

.project-description {
  font-size: 1rem;
}

.project-languages {
  display: flex;
  flex-direction: row;
}

.github-link {
  margin-left: 14rem;
}
</style>
