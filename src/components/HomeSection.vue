<template>
  <section id="home">
    <div class="intro">
      <div class="wrap">
        <div class="content">
          <img src="/img/fotoAvatar.png" alt="foto perfil" class="fotoPerfil" />
          <div class="text">
            <h1>Front-End Developer 👨🏻‍💻</h1>
            <p>
              👋🏻 Hello World, I'm Leonardo Cordeiro. A passionate Front-End Developer <br />
              based in Rio de Janeiro, Brazil. 🇧🇷
            </p>
            <div class="icons">
              <button>
                <a href="mailto:gama05596@gmail.com" target="_blank">
                  <img src="/icons/icons8-gmail-logo.svg" alt="" />
                </a>
              </button>
              <button>
                <a href="https://wa.me/5521968437171" target="_blank">
                  <img src="/icons/icons8-whatsapp.svg" alt="" />
                </a>
              </button>
              <button>
                <a href="https://www.linkedin.com/in/leonardo-cordeiro28/" target="_blank">
                  <img src="/icons/icons8-linkedin.svg" alt="" />
                </a>
              </button>
              <button>
                <a href="https://github.com/leonardo-cordeiro" target="_blank">
                  <img src="/icons/icons8-github.svg" alt="" />
                </a>
              </button>
            </div>
          </div>
        </div>
        <LanguageCardVue />
      </div>
    </div>
  </section>
</template>

<script setup>
import LanguageCardVue from './LanguageCard.vue'
</script>

<style scoped>
.intro {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #91ac9a;
  height: 100vh;
  padding-top: 2rem;
  width: 100%;
}

.wrap {
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: space-around;
  align-items: center;
}

.content {
  display: flex;
  flex-direction: column;
  text-align: center;
  justify-content: center;
  align-items: center;
  margin-top: 4rem;
}

.text p {
  font-size: 1.1rem;
  white-space: pre-line;
  font-family: Arial, Helvetica, sans-serif;
  /* color: white; */
  color: rgb(0, 0, 0);
}

.text h1 {
  font-size: 3rem;
  font-family: 'Poppins', sans-serif;
  font-weight: 700;
  /* color: white; */
  color: #262626e3;
}

.fotoPerfil {
  width: 230px;
  /* margin-top: 3rem; */
  /* background-color: #6d9cf3dc; */
  border: 1.5px solid #b9b9b950;
  border-radius: 30%;
}

.icons {
  display: flex;
  justify-content: center;
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
    /* gap: 2rem; */
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
    /* margin-top: 2rem; */
    justify-content: center;
  }
  .content {
    margin-top: 1rem;
  }
}
</style>
