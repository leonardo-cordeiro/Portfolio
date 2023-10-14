<template>
  <section id="home">
    <div class="intro">
      <div class="wrap">
        <img src="src/img/fotoAvatar.png" alt="foto perfil" class="fotoPerfil" />
        <div class="text">
          <h1>Front-End Developer 👨🏻‍💻</h1>
          <p>
            👋🏻 Hello World, I'm Leonardo Cordeiro. A passionate Front-End Developer <br />
            based in Rio de Janeiro, Brazil. 🇧🇷
          </p>
          <div class="icons">
            <button>
              <a href="mailto:gama05596@gmail.com" target="_blank">
                <img src="src/icons/icons8-gmail-logo.svg" alt="" />
              </a>
            </button>
            <button>
              <a href="https://wa.me/5521968437171" target="_blank">
                <img src="src/icons/icons8-whatsapp.svg" alt="" />
              </a>
            </button>
            <button>
              <a href="https://www.linkedin.com/in/leonardo-cordeiro28/" target="_blank">
                <img src="src/icons/icons8-linkedin.svg" alt="" />
              </a>
            </button>
            <button>
              <a href="https://github.com/leonardo-cordeiro" target="_blank">
                <img src="src/icons/icons8-github.svg" alt="" />
              </a>
            </button>
          </div>
        </div>
      </div>
      <!-- <CarrouselSection /> -->
    </div>
  </section>
</template>

<script setup>
// import CarrouselSection from '@/components/CarrouselSection.vue'
</script>

<style scoped>
.intro {
  display: flex;
  flex-direction: column;
  align-items: center;
  background: linear-gradient(135deg, #3403b7 31%, #07034d 80%);
  height: 100vh;
  padding-top: 5rem;
  width: 100%;
}

.wrap {
  gap: 10rem;
  margin: 2rem auto;
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
  width: 280px;
  margin-top: 3rem;
  background-color: #6d9cf3dc;
  border: 1.5px solid #b9b9b950;
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

@media screen and (max-width: 767px) {
  .intro {
    /* padding: 5rem 2rem; */
    text-align: center;
  }

  .wrap {
    flex-direction: column;
    gap: 2rem;
  }

  .text p {
    font-size: 1rem;
  }

  .text h1 {
    font-size: 2rem;
    margin-bottom: 1rem;
  }

  .fotoPerfil {
    width: 200px;
    margin-top: 2rem;
  }
  .icons {
    margin-top: 2rem;
    justify-content: center;
  }
}
</style>
