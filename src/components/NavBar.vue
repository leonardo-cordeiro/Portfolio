<template>
  <header class="header-area">
    <div class="navbar-area">
      <div class="container">
        <nav class="site-navbar">
          <a href="#home" class="site-logo">Leonardo.dev</a>
          <ul :class="{ open: isNavOpen }">
            <li @click="closeToggle"><a href="#home">home</a></li>
            <li @click="closeToggle"><a href="#about">about</a></li>
            <li @click="closeToggle"><a href="#portfolio">portfolio</a></li>
          </ul>
          <button class="nav-toggler" @click="toggleNav">
            <span :class="{ 'toggler-open': isNavOpen }"></span>
          </button>
        </nav>
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue'

const isNavOpen = ref(false)

function toggleNav() {
  isNavOpen.value = !isNavOpen.value
}

function closeToggle() {
  isNavOpen.value = false
}
</script>

<style scoped>
.container {
  width: 100%;
  margin: 0 auto;
  padding: 0 15px;
  position: fixed;
  /* background: linear-gradient(135deg, #3403b7 31%, #07034d 80%); */
  z-index: 9999;
  background-color: #cedfdf;
}

.site-navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
a.site-logo {
  font-size: 30px;
  font-weight: 800;
  color: rgb(72, 72, 72);
  text-decoration: none;
  margin-left: 2rem;
}
.site-navbar ul {
  margin: 0 2rem;
  padding: 0;
  list-style: none;
  display: flex;
}
.site-navbar ul li a {
  color: rgb(72, 72, 72);
  padding: 20px;
  display: block;
  text-decoration: none;
  text-transform: uppercase;
}
.site-navbar ul li a:hover {
  text-decoration: underline;
  color: #f2f2f2e2;
}

.nav-toggler {
  border: 3px solid #fff;
  padding: 5px;
  background-color: transparent;
  cursor: pointer;
  height: 39px;
  display: none;
}
.nav-toggler span,
.nav-toggler span:before,
.nav-toggler span:after {
  width: 28px;
  height: 3px;
  background-color: #fff;
  display: block;
  transition: 0.3s;
}
.nav-toggler span:before {
  content: '';
  transform: translateY(-9px);
}
.nav-toggler span:after {
  content: '';
  transform: translateY(6px);
}
.nav-toggler.toggler-open span {
  background-color: transparent;
}
.nav-toggler.toggler-open span:before {
  transform: translateY(0px) rotate(45deg);
}
.nav-toggler.toggler-open span:after {
  transform: translateY(-3px) rotate(-45deg);
}

@media screen and (max-width: 767px) {
  .container {
    max-width: 720px;
    padding: 0;
  }

  .nav-toggler {
    display: block;
    margin-right: 1rem;
  }
  .site-navbar {
    min-height: 60px;
  }
  .site-navbar ul {
    position: absolute;
    width: 100%;
    height: calc(100vh - 60px);
    left: 0;
    top: 60px;
    flex-direction: column;
    align-items: center;
    border-top: 1px solid #444;
    background-color: rgba(255, 255, 255, 0.89);
    max-height: 0;
    overflow: hidden;
    transition: 0.3s;
    margin: 0;
  }
  .site-navbar ul li {
    width: 100%;
    text-align: center;
  }
  .site-navbar ul li a {
    padding: 25px;
  }
  .site-navbar ul li a:hover {
    background-color: rgba(255, 255, 255, 0.1);
  }
  .site-navbar ul.open {
    max-height: 100vh;
    overflow: visible;
  }
  .intro-area h2 {
    font-size: 36px;
    margin-bottom: 15px;
  }
  a.site-logo {
    margin: 0 1rem;
  }
}
</style>
