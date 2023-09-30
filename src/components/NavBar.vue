<template>
  <header>
    <nav>
      <h3>Leonardo.dev</h3>
      <ul class="socialMedia">
        <li v-for="item in menuItems" :key="item">{{ item }}</li>
      </ul>
    </nav>
  </header>
</template>

<script setup>
import { ref } from 'vue'

const menuItems = ref(['Home', 'About', 'Portfolio'])
</script>

<style scoped>
header {
  padding: 10px 20px;
  /* color: #0084a8; */
  color: #fff;
  font-family: 'Poppins', 'sans-serif';
}

nav {
  display: flex;
  align-items: center;
  justify-content: space-around;
  width: 100%;
  padding: 25px 40px 25px 50px;
  background: linear-gradient(135deg, #3403b7 31%, #07034d 80%);
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 200;
}

nav h3 {
  margin: 0;
  padding: 0;
  font-size: 24px;
  font-weight: 900;
  margin-right: 30rem;
  order: 1;
}

ul.socialMedia {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  order: 2;
}

ul.socialMedia li {
  margin-left: 20px;
  font-size: 16px;
  font-weight: 600;
  padding: 0.5rem;
  cursor: pointer;
}

ul.socialMedia li:hover {
  color: #c0c0c0;
  /* padding: 0.5rem; */
  border-radius: 10%;
}
</style>
