<template>
  <main>
    <!-- Cabeçalho -->
    <NavBar />

    <!-- Introdução -->
    <HomeSection />

    <TesteCarrousel />
    <!-- About  -->
    <AboutSectionVue />

    <!-- Portfolio -->
    <PortfolioSectionVue />

    <!-- Footer -->
    <FooterSection />
  </main>
</template>

<script setup>
import AboutSectionVue from '@/components/AboutSection.vue'
import HomeSection from '@/components/HomeSection.vue'
import NavBar from '@/components/NavBar.vue'
import PortfolioSectionVue from '@/components/PortfolioSection.vue'
import FooterSection from './components/FooterSection.vue'
import TesteCarrousel from './components/TesteCarrousel.vue'
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Fira+Sans:ital,wght@0,200;0,500;1,700&family=Poppins:wght@100;300;400&display=swap');

/* Reset de margem e preenchimento padrão */
html,
body {
  margin: 0;
  padding: 0;
  scroll-behavior: smooth;
}

/* Estilos globais */
body {
  background: white;
  font-family: 'Poppins', sans-serif;
  color: #4d4d4d;
  line-height: 1.5;
}
</style>
