<template>
  <div class="wrap">
    <div class="buttons">
      <button class="portfolio-button">Portfolio</button>
      <button class="freelancer-button">Freelancer</button>
    </div>
    <div class="base-cards-carousel">
      <div class="base-cards-container">
        <!-- Repita para cada BaseCard -->
        <BaseCard
          link="https://brasileiro.ninja/"
          img="src/img/brasileiroNinja.png"
          title="Brasileiro Ninja"
          description="Site para fazer diversas pesquisas, como: Tabela Fipe, Feriados, CNPJ..."
          vue="true"
          javascript="true"
        />
        <BaseCard
          link="https://brasileiro.ninja/"
          img="src/img/brasileiroNinja.png"
          title="Brasileiro Ninja"
          description="Site para fazer diversas pesquisas, como: Tabela Fipe, Feriados, CNPJ..."
          vue="true"
          javascript="true"
        />
        <BaseCard
          link="https://brasileiro.ninja/"
          img="src/img/brasileiroNinja.png"
          title="Brasileiro Ninja"
          description="Site para fazer diversas pesquisas, como: Tabela Fipe, Feriados, CNPJ..."
          vue="true"
          javascript="true"
        />
        <BaseCard
          link="https://brasileiro.ninja/"
          img="src/img/brasileiroNinja.png"
          title="Brasileiro Ninja"
          description="Site para fazer diversas pesquisas, como: Tabela Fipe, Feriados, CNPJ..."
          vue="true"
          javascript="true"
        />
        <BaseCard
          link="https://brasileiro.ninja/"
          img="src/img/brasileiroNinja.png"
          title="Brasileiro Ninja"
          description="Site para fazer diversas pesquisas, como: Tabela Fipe, Feriados, CNPJ..."
          vue="true"
          javascript="true"
        />
        <BaseCard
          link="https://brasileiro.ninja/"
          img="src/img/brasileiroNinja.png"
          title="Brasileiro Ninja"
          description="Site para fazer diversas pesquisas, como: Tabela Fipe, Feriados, CNPJ..."
          vue="true"
          javascript="true"
        />
        <!-- Repita para cada BaseCard -->
      </div>
    </div>
  </div>
</template>

<script setup>
import BaseCard from './BaseCard.vue'
</script>

<style scoped>
.wrap {
  padding: 3rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #386fded0;
  height: 100%;
}

.buttons {
  display: flex;
  gap: 10px; /* Espaço entre os botões */
  margin-bottom: 1rem; /* Espaçamento entre botões e Carrossel */
}

button {
  padding: 10px 20px; /* Espaçamento interno do botão */
  border: none;
  background-color: #007bff; /* Cor de fundo */
  color: #fff; /* Cor do texto */
  cursor: pointer;
  font-size: 18px; /* Tamanho da fonte */
  border-radius: 5px; /* Cantos arredondados */
  transition: background-color 0.3s ease; /* Transição suave da cor de fundo */
}

/* Estilo quando o cursor passa sobre os botões */
button:hover {
  background-color: #0056b3; /* Cor de fundo alterada no hover */
}

/* Estilos específicos para cada botão */
.portfolio-button {
  background-color: #007bff; /* Cor de fundo para o botão "Portfolio" */
}

.freelancer-button {
  background-color: #6c757d; /* Cor de fundo para o botão "Freelancer" */
}

.base-cards-carousel {
  overflow: hidden;
  width: 100%; /* Largura do Carrossel */
  margin: 0 auto;
}

.base-cards-container {
  display: flex;
  flex-wrap: wrap; /* Permite que as BaseCards quebrem para a próxima linha */
  justify-content: space-between; /* Espaçamento igual entre as BaseCards */
}
.base-cards-container .base-card {
  flex: 0 0 calc(20% - 20px); /* Largura de cada BaseCard (altere o valor 20% para ajustar o tamanho) */
  margin-right: 20px; /* Espaçamento entre os BaseCards */
  margin-bottom: 20px; /* Espaçamento abaixo das linhas de BaseCards */
}

/* Ajuste a altura dos BaseCards conforme necessário */
.base-cards-container .base-card img {
  height: 100px; /* Altura dos BaseCards */
}
</style>
