<template>
  <section class="about-section" id="about">
    <div class="container">
      <div class="about-content">
        <div class="about-text">
          <h2>A Small Piece of My History...</h2>
          <p>
            I am a determined Brazilian, who does not let obstacles get me down. Programming was a
            challenge that I faced with courage and dedication, until I became a competent and
            passionate professional. Today, I live for the code and have fun with the projects and
            challenges that it offers me.
          </p>
          <p>
            My life was also marked by other experiences that made me grow. I practiced track and
            field professionally. I lived in the United States for a few years, learning a new
            language and a new culture. I traveled across Brazil, being amazed by its landscapes and
            its people. My journey is a combination of determination, programming and adventure.
          </p>
          <!-- <button class="resume">
            <a href="public/pdf/resumeCV.pdf" download> Dowload Resume</a>
            <div>
              <img class="resume_img" src="/icons/resume.png" alt="resume icon" />
            </div>
          </button> -->
        </div>
        <div class="about-image">
          <img src="/img/foto_about.jpg" alt="Leonardo Gama" />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
.about-section {
  padding: 80px 0;
  text-align: center;
  background-color: #a9c3b6;
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
  color: #262626ba;
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
  max-width: 470px;
  border-radius: 10px;
  margin-top: 20px;
  margin-left: 10rem;
  background-color: #000000b7;
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
