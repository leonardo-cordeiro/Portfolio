<template>
  <section>
    <div class="intro">
      <div class="wrap">
        <img src="src/img/fotoAvatar.png" alt="foto perfil" class="fotoPerfil" />
        <div class="text">
          <h1>Front-End Vue.js Developer 👾</h1>
          <p>
            👋🏻 Hello World, I'm Leonardo Cordeiro. A passionate Front-End Vue.js Developer <br />
            based in Rio de Janeiro, Brazil. 🇧🇷
          </p>
          <div class="icons">
            <button>
              <a href="" target="_blank">
                <img src="src/icons/icons8-gmail-logo.svg" alt="" />
              </a>
            </button>
            <button>
              <a href="" target="_blank">
                <img src="src/icons/icons8-whatsapp.svg" alt="" />
              </a>
            </button>
            <button>
              <a href="" target="_blank">
                <img src="src/icons/icons8-linkedin.svg" alt="" />
              </a>
            </button>
            <button>
              <a href="" target="_blank">
                <img src="src/icons/icons8-github.svg" alt="" />
              </a>
            </button>
          </div>
        </div>
      </div>
      <CarrouselSection />
    </div>
  </section>
</template>

<script setup>
import CarrouselSection from './CarrouselSection.vue'
</script>

<style scoped>
.intro {
  display: flex;
  flex-direction: column;
  align-items: center;
  background: linear-gradient(135deg, #00c6fb 31%, #005bea 80%);
  height: 100vh;
  padding-top: 5rem;
  width: 100%;
}

.wrap {
  display: flex;
  align-items: center;
  gap: 10rem;
}

.text p {
  font-size: 1.1rem;
  white-space: pre-line;
  font-family: Arial, Helvetica, sans-serif;
  color: white;
}

.text h1 {
  font-size: 3rem;
  font-family: 'Poppins', sans-serif;
  font-weight: 700;
  color: white;
}

.fotoPerfil {
  width: 320px;
  margin-top: 3rem;
  background-color: #8ce0ffaf;
  border: 1.5px solid #b9b9b9;
  border-radius: 30%;
}

.icons {
  display: flex;
}

button {
  background: transparent;
  border: none;
  margin: 5px;
}
</style>
