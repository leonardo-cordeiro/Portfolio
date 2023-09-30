<template>
  <div class="wrap">
    <div class="buttons">
      <button @click="onClickShowPortfolio" class="portfolio-button">Portfolio</button>
      <button @click="onClickShowFreelancer" class="freelancer-button">Freelancer</button>
    </div>

    <div v-if="showPortfolio" class="base-cards-container">
      <BaseCard
        link="https://brasileiro.ninja/"
        img="src/img/brasileiroNinja.png"
        title="Brasileiro Ninja"
        description="Site para fazer diversas pesquisas, como: Tabela Fipe, Feriados, CNPJ..."
        vue="true"
        javascript="true"
        github="true"
        github_link="https://github.com/leonardo-cordeiro"
      />
      <BaseCard
        link="https://brasileiro.ninja/"
        img="src/img/brasileiroNinja.png"
        title="Brasileiro Ninja"
        description="Site para fazer diversas pesquisas, como: Tabela Fipe, Feriados, CNPJ..."
        vue="true"
        javascript="true"
        github="true"
        github_link="https://github.com/leonardo-cordeiro"
      />
      <BaseCard
        link="https://brasileiro.ninja/"
        img="src/img/crypto_Tracker.png"
        title="Crypto Tracker"
        description="Cryptocurrency website, with daily variation in coin prices and user authentication."
        vue="true"
        javascript="true"
        github="true"
        github_link="https://github.com/leonardo-cordeiro"
      />
      <BaseCard
        link=""
        img="src/img/Finance_App.png"
        title="Finance App"
        description="Expense tracking website, which has a graph showing the balance and a transaction history"
        vue="true"
        javascript="true"
        github="true"
        github_link="https://github.com/leonardo-cordeiro"
      />
      <BaseCard
        link="https://weather-app-7tx.pages.dev/"
        img="src/img/weather_app.png"
        title="Weather App"
        description="Weather forecast website for any city in the world"
        javascript="true"
        html="true"
        github="true"
        github_link="https://github.com/leonardo-cordeiro"
      />
      <BaseCard
        link="https://b62d5232.calculadora-de-juros-compostos.pages.dev/"
        img="src/img/calculadora_juros_compostos.png"
        title="Compound interest calculator"
        description="Calculates compound interest according to the amount and time entered"
        javascript="true"
        html="true"
        github="true"
        github_link="https://github.com/leonardo-cordeiro"
      />
    </div>

    <div v-if="showFreelancer" class="base-cards-container">
      <BaseCard
        link="https://patronotransportes.com/"
        img="src/img/patrono_freelancer.png"
        title="Patrono Transportes"
        description="Site para fazer diversas pesquisas, como: Tabela Fipe, Feriados, CNPJ..."
        vue="true"
        javascript="true"
        web="true"
        web_link="https://patronotransportes.com/"
      />
      <BaseCard
        link="http://www.rendaz.com.br/wtorre/"
        img="src/img/Captura de Tela 2023-09-29 às 18.09.33.png"
        title="W-torre Engenharia"
        description="Site para fazer diversas pesquisas, como: Tabela Fipe, Feriados, CNPJ..."
        vue="true"
        javascript="true"
        web="true"
        web_link="http://www.rendaz.com.br/wtorre/"
      />
    </div>
  </div>
</template>

<script setup>
import BaseCard from './BaseCard.vue'
import { ref } from 'vue'

const showPortfolio = ref(true)
const showFreelancer = ref(false)

function onClickShowPortfolio() {
  showPortfolio.value = true
  showFreelancer.value = false
}

function onClickShowFreelancer() {
  showPortfolio.value = false
  showFreelancer.value = true
}
</script>

<style scoped>
.wrap {
  padding: 3rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #4800d9;
  height: 100%;
}

.buttons {
  display: flex;
  gap: 10px;
  margin-bottom: 1rem;
}

button {
  padding: 10px 30px;
  border: none;
  background: #007bff;
  color: #fff;
  cursor: pointer;
  font-size: 18px;
  border-radius: 5px;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #0056b3;
}

.portfolio-button {
  background-color: #007bff;
}

.freelancer-button {
  background-color: #6c757d;
}

.base-cards-container {
  display: flex;
  flex-wrap: wrap;
}
</style>
