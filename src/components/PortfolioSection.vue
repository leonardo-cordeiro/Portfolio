<template>
  <div class="wrap" id="portfolio">
    <div class="buttons">
      <button @click="toggleSection('portfolio')" :class="{ active: isActive('portfolio') }">
        Portfolio
      </button>
      <button @click="toggleSection('freelancer')" :class="{ active: isActive('freelancer') }">
        Freelancer
      </button>
    </div>

    <div v-if="isActive('portfolio')" class="base-cards-container">
      <BaseCard
        link="https://brasileiro.ninja/"
        img="/img/brasileiroNinja.png"
        title="Brasileiro Ninja"
        description="Site para fazer diversas pesquisas, como: Tabela Fipe, Feriados, CNPJ..."
        vue="true"
        javascript="true"
        chartjs="true"
        github="true"
        github_link="https://github.com/arnonrdp/Brasileiro-Ninja"
      />
      <BaseCard
        link="https://cryptotracker-5hk.pages.dev/"
        img="/img/crypto_Tracker.png"
        title="Crypto Tracker"
        description="Cryptocurrency website, with daily variation in coin prices."
        vue="true"
        javascript="true"
        github="true"
        firebase="true"
        tailwind="true"
        github_link="https://github.com/leonardo-cordeiro/CryptoTracker"
      />
      <BaseCard
        link=""
        img="/img/Finance_App.png"
        title="Finance App"
        description="Expense tracking website, which has a graph showing the balance and a transaction history"
        vue="true"
        javascript="true"
        github="true"
        chartjs="true"
        github_link="https://github.com/leonardo-cordeiro/finance-app-vue"
      />
      <BaseCard
        link="https://leonardodev.pages.dev/"
        img="/img/Captura de Tela 2023-10-14 às 15.16.41.png"
        title="Personal Portfolio"
        description="This is my portfolio page to present my professional and personal projects"
        vue="true"
        javascript="true"
        css="true"
        github="true"
        github_link="https://github.com/leonardo-cordeiro"
      />

      <BaseCard
        img="/img/Captura de Tela 2023-10-14 às 15.03.30.png"
        title="Python Web Scraping"
        description="Web Scraping using python integrated with MySql data base"
        python="true"
        mysql="true"
        github="true"
        github_link="https://github.com/leonardo-cordeiro/Web-Scraping-python"
      />

      <BaseCard
        link="https://weather-app-7tx.pages.dev/"
        img="/img/weather_app.png"
        title="Weather App"
        description="Weather forecast website where you can check the weather"
        javascript="true"
        html="true"
        css="true"
        github="true"
        github_link="https://github.com/leonardo-cordeiro/projeto-weather"
      />
      <BaseCard
        link="https://b62d5232.calculadora-de-juros-compostos.pages.dev/"
        img="/img/calculadora_juros_compostos.png"
        title="Compound interest calculator"
        description="Calculates compound interest according to the amount and time entered"
        javascript="true"
        html="true"
        css="true"
        github="true"
        github_link="https://github.com/leonardo-cordeiro/calculadora-de-juros-compostos"
      />
    </div>

    <div v-if="isActive('freelancer')" class="base-cards-container">
      <BaseCard
        link="https://patronotransportes.com/"
        img="/img/patrono_freelancer.png"
        title="Patrono Transportes"
        description="Landing page for a transport company, with a gallery of photos and a contact form."
        javascript="true"
        html="true"
        css="true"
        php="true"
        web="true"
        web_link="https://patronotransportes.com/"
      />
      <BaseCard
        link="http://www.rendaz.com.br/wtorre/"
        img="/img/Captura de Tela 2023-09-29 às 18.09.33.png"
        title="W-torre Engenharia"
        description="Landing page for a construction company, with a gallery of photos and a contact form."
        javascript="true"
        html="true"
        css="true"
        php="true"
        web="true"
        web_link="http://www.rendaz.com.br/wtorre/"
      />
      <BaseCard
        link="https://golfim.com.br/"
        img="/img/golfim_freelancer.png"
        title="Golfim Piscinas"
        description="Landing page for a pool company, with a contact form and a gallery of photos."
        javascript="true"
        html="true"
        css="true"
        vue="true"
        web="true"
        web_link="https://golfim.com.br/"
      />
    </div>
  </div>
</template>

<script setup>
import BaseCard from '@/components/BaseCard.vue'
import { ref } from 'vue'

const activeSection = ref('portfolio')

const toggleSection = (section) => (activeSection.value = section)

const isActive = (section) => activeSection.value === section
</script>

<style scoped>
.wrap {
  padding: 3rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  /* background-color: #4800d9; */
  height: 100%;
  background-color: #b7d1d3;
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

.base-cards-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.active {
  background-color: #ccc;
}
</style>
