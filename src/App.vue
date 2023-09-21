<template>
  <main>
    <!-- Cabeçalho -->
    <NavBar />

    <!-- Introdução -->
    <HomeSection />

    <!-- About  -->
    <AboutSectionVue />
  </main>
</template>

<script setup>
import AboutSectionVue from '@/components/AboutSection.vue'
import HomeSection from '@/components/HomeSection.vue'
import NavBar from '@/components/NavBar.vue'
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Fira+Sans:ital,wght@0,200;0,500;1,700&family=Poppins:wght@100;300;400&display=swap');

/* Reset de margem e preenchimento padrão */
html,
body {
  margin: 0;
  padding: 0;
}

/* Estilos globais */
body {
  background: white;
  font-family: 'Poppins', sans-serif;
  color: #4d4d4d;
}
</style>
