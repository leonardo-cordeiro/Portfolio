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
        <a v-if="github" :href="github_link" class="github-link language" target="_blank">
          <LanguageIcon icon="src/icons/icons8-github.svg" alt="Github icon" />
        </a>

        <a v-if="web" :href="web_link" class="github-link language" target="_bank">
          <LanguageIcon icon="src/icons/icons8-website-50.png" alt="Web Icon" />
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
import LanguageIcon from '@/components/LanguageIcon.vue'

defineProps({
  title: String,
  description: String,
  img: String,
  html: Boolean,
  css: Boolean,
  javascript: Boolean,
  vue: Boolean,
  link: String,
  github: Boolean,
  github_link: String,
  web: Boolean,
  web_link: String
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
  max-height: 400px;
  width: 30%;
  height: 100%;
  background-color: #f2f2f2;
}

.project-img {
  max-height: 200px;
  width: 100%;
  cursor: pointer;
}

.project-details {
  padding-left: 10px;
  padding-right: 5px;
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
  margin-left: 15rem;
}
</style>
