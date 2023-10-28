<template>
  <div class="wrap">
    <div class="card">
      <LanguageIconCard icon="/icons/icons8-html-5-240.svg" alt="HTML" />
      <LanguageIconCard icon="/icons/css-3.png" alt="CSS" />
      <LanguageIconCard icon="/icons/icons8-javascript-240.png" alt="JavaScript" />
      <LanguageIconCard icon="/icons/icons8-vue-js.svg" alt="Vue.js" />
      <LanguageIconCard icon="/icons/chart-js-seeklogo.com.svg" alt="Chart.js" />
      <LanguageIconCard icon="/icons/icons8-bootstrap.svg" alt="Bootstrap" />
      <LanguageIconCard icon="/icons/quasar-svgrepo-com.svg" alt="Quasar" />
      <LanguageIconCard icon="/icons/tailwindcss-icon.svg" alt="Tailwind" />
      <LanguageIconCard icon="/icons/icons8-firebase.svg" alt="Firebase" />
      <LanguageIconCard icon="/icons/python-icon.svg" alt="Python" />
      <LanguageIconCard icon="/icons/icons8-mysql-logo.svg" alt="MySql" />
    </div>
  </div>
</template>

<script setup>
import LanguageIconCard from '@/components/LanguageIconCard.vue'

defineProps({
  alt: String
})
</script>

<style scoped>
.wrap {
  display: flex;
  flex-direction: column;
}

.card {
  width: 100%;
  border: 1px solid #ddd;
  border-radius: 20px;
  padding: 10px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  background-color: #bbecdf6b;
  margin-top: 3rem;
  z-index: 1;
}

.card img {
  width: 60px;
  height: 60px;
  object-fit: cover;
  border-radius: 10px;
  margin: 0 15px 10px 0;
  background: #fffdfd82;
}

.card img:hover {
  cursor: pointer;
  transform: scale(1.1);
  transition: all 0.2s ease-in-out;
}
</style>
