<template>
  <section class="about-section" id="about">
    <div class="container">
      <div class="about-content">
        <div class="about-text">
          <h2>Olá, sou Leonardo Gama</h2>
          <p>
            Sou um apaixonado por desenvolvimento Front-End, criando experiências digitais incríveis
            com Vue.js.
          </p>
          <p>
            Minha jornada no mundo da tecnologia é impulsionada pela determinação, foco inabalável e
            paixão por colaborar em equipe. Com experiência adquirida em quase três anos nos Estados
            Unidos, alcancei um alto nível de proficiência em inglês. Além de codificar, minha
            dedicação à colaboração e minha perspectiva global me permitem interagir eficazmente com
            diversas partes interessadas.
          </p>
          <p>
            Sou um solucionador de problemas entusiasmado, sempre em busca de novos desafios e
            projetos inovadores. Estou pronto para contribuir com minha experiência e paixão para o
            campo em constante evolução do desenvolvimento Front-End.
          </p>
          <button class="resume">
            <a href="src/pdf/ProfileEnglish.pdf" download> Dowload Resume</a>
            <div>
              <img class="resume_img" src="src/icons/resume (1).png" alt="resume icon" />
            </div>
          </button>
        </div>
        <div class="about-image">
          <img src="src/img/foto_about.jpg" alt="Leonardo Gama" />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
.about-section {
  background-color: #3b1cb7;
  padding: 80px 0;
  text-align: center;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
}

.about-content {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  color: #ffff;
}

.about-text {
  text-align: left;
  max-width: 500px;
  margin-right: 30px;
}

.about-text h2 {
  font-size: xx-large;
}
.about-text p {
  font-size: large;
}

.about-image img {
  width: 100%;
  max-width: 550px;
  border-radius: 10px;
  margin-top: 20px;
  margin-left: 10rem;
}

.resume {
  padding: 15px 30px;
  border-radius: 30px;
  background-color: #007bff40;
  color: #fff;
  font-size: 1.2rem;
  border: none;
  cursor: pointer;
  transition: background-color 0.3s ease;
  margin-top: 25px;
  display: flex;
}

.resume:hover {
  background-color: #0056b3;
}

.resume a {
  text-decoration: none;
  color: #fff;
}

.resume_img {
  margin-left: 8px;
  width: 25px;
}
</style>
