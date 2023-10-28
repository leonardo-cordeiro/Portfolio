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
        <div style="display: flex">
          <LanguageIcon v-if="vue" icon="/icons/icons8-vue-js.svg" alt="Vue" />
          <LanguageIcon
            v-if="javascript"
            icon="/icons/icons8-javascript-240.png"
            alt="JavaScript"
          />
          <LanguageIcon v-if="css" icon="/icons/css-3.svg" alt="CSS" />
          <LanguageIcon v-if="html" icon="/icons/icons8-html-5-240.svg" alt="HTML" />
          <LanguageIcon v-if="chartjs" icon="/icons/chart-js-seeklogo.com.svg" alt="Chart.js" />
          <LanguageIcon v-if="firebase" icon="/icons/icons8-firebase.svg" alt="Firebase" />
          <LanguageIcon v-if="tailwind" icon="/icons/tailwindcss-icon.svg" alt="Tailwind" />
          <LanguageIcon v-if="python" icon="/icons/python-icon.svg" alt="Python" />
          <LanguageIcon v-if="mysql" icon="/icons/icons8-mysql-logo.svg" alt="MySql" />
          <LanguageIcon v-if="php" icon="/icons/php-icon.svg" alt="php" />
          <LanguageIcon v-if="quasar" icon="/icons/quasar-svgrepo-com.svg" alt="php" />
        </div>
        <div>
          <a v-if="github" :href="github_link" class="github-link language" target="_blank">
            <LanguageIcon icon="/icons/icons8-github.svg" alt="Github" />
          </a>

          <a v-if="web" :href="web_link" class="github-link language" target="_bank">
            <LanguageIcon icon="/icons/icons8-website-50.png" alt="Web Icon" />
          </a>
        </div>
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
  chartjs: Boolean,
  css: Boolean,
  javascript: Boolean,
  vue: Boolean,
  firebase: Boolean,
  link: String,
  github: Boolean,
  github_link: String,
  web: Boolean,
  web_link: String,
  tailwind: Boolean,
  python: Boolean,
  mysql: Boolean,
  php: Boolean,
  quasar: Boolean
})
</script>

<style scoped>
.project-card {
  margin: 15px;
  border: 2px solid #fff;
  border-radius: 12px;
  transition: all 0.2s ease-in-out;
  display: flex;
  flex-direction: column;
  width: 25%;
  background-color: #f2f2f2;
}

.project-card:hover {
  scale: 1.02;
  box-shadow: 10px 10px #00000057;
}

.project-img {
  max-height: 200px;
  width: 100%;
  cursor: pointer;
  border-radius: 12px 12px 0 0;
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
  justify-content: space-between;
  z-index: 1;
}

@media screen and (max-width: 767px) {
  .project-card {
    width: 400px;
    max-width: 90vw;
  }
}

@media only screen and (min-width: 768px) and (max-width: 1024px) {
  .project-card {
    width: 325px;
    max-width: 90vw;
  }
}
</style>
