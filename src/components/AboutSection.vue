<template>
  <section class="about-section" id="about">
    <div class="container">
      <div class="about-content">
        <div class="about-text">
          <h2>A Small Piece of My History...</h2>
          <p>
            I am Brazilian, and like many compatriots, I have that unwavering determination that
            characterizes us. When I began my journey in programming, there were moments when I
            thought about giving up, but as a good Brazilian, that simply isn't an option for me.
            After a long period of study and dedication, I finally realized that I was making
            significant progress in the world of programming and was truly getting the hang of it.
            Today, my passion for programming only increases, and I don't go a day without immersing
            myself in code.
          </p>
          <p>
            Beyond programming, I was a professional athlete in track and field, and I lived in the
            United States for nearly three years, enriching my worldview. Traveling throughout
            Brazil allowed me to get to know its diverse regions and incredible people. My journey
            is a blend of determination, a passion for programming, and a constant desire to explore
            new horizons.
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

@media screen and (max-width: 767px) {
  .about-content {
    display: flex;
    flex-direction: column;
    text-align: center;
    align-items: center;
  }

  .about-image img {
    display: none;
  }

  .about-text {
    margin: 10px;
  }
}

@media screen and (min-width: 768px) and (max-width: 1024px) {
  .about-content {
    display: grid;
    grid-template-columns: repeat(auto, minmax(calc((100% - calc(((100vw / 1)))))));
    grid-gap: var(--space);
    justify-content: space-evenly;
  }

  .about-image img {
    max-width: 70vw;
    align-items: center;
    margin-left: 0;
  }
}
</style>
