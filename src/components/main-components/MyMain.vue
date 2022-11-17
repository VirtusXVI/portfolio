<template>
  <main>
    <!-- ABOUT SECTION -->
    <section id="about-section" class="about-section">
      <div class="small-logo">

      </div>
      <div class="about-title">
        Ciao, sono Manuel. Sono un Full-Stack web developer
      </div>
      <div>
        <img class="img" src='../../assets/img/me.jpg' alt="me">
      </div>
      <div class="discover-text">
        <a href="#">
          Scopri cosa so fare<br>
          <i class="fa-solid fa-chevron-down"></i>
        </a>
      </div>
    </section>
    <!-- SKILLS SECTION -->
    <section id="skills-section" class="skills-section">
      <div class="titles">
        LE MIE SKILLS
      </div>
      <!-- CARDS -->
      <div class="skills-cards">
        <!-- FIRST CARD -->
        <div class="skill-card">
          <img class="tech-icon" src="../../assets/img/frontend.png" alt="">
          <h2>FRONT END DEVELOPMENT</h2>
          <ul>
            <li>HTML 5</li>
            <li>CSS 3</li>
            <li>JAVASCRIPT</li>
            <li>VUE.JS</li>
          </ul>
        </div>
        <!-- SECOND CARD -->
        <div class="skill-card">
          <img class="tech-icon" src="../../assets/img/backend.jpg" alt="">
          <h2>BACK END DEVELOPMENT</h2>
          <ul>
            <li>PHP</li>
            <li>LARAVEL</li>
          </ul>
        </div>
        <!-- THIRD CARD -->
        <div class="skill-card">
          <img class="tech-icon" src="../../assets/img/tools.jpg" alt="">
          <h2>DEV TOOLS</h2>
          <ul>
            <li>BOOTSTRAP</li>
            <li>GITHUB</li>
            <li>GIT</li>
            <li>VS CODE</li>
          </ul>
        </div>
      </div>
    </section>
    <!-- PROJECTS SECTION -->
    <section id="projects-section" class="projects-section">
      <div class="titles">
        I MIEI PROGETTI
      </div>
      <div class="projects-cards">
        <!-- FIRST CARD -->
        <div class="project-card">
          <img src="../../assets/img/projects/boolflix.png" alt="">
          <div>
            Progetto riguardante l'utilizzo di API per ricevere dati da un database e mostrarli in pagina.
          </div>
        </div>
        <!-- SECOND CARD -->
        <div class="project-card">
          <img src="../../assets/img/projects/deliveboo.png" alt="">
          <div>
            Progetto di gruppo il cui obiettivo era quello di riprodurre un sistema simile a quello di Deliveroo gestendo i ristoranti,gli ordini e i pagamenti.
          </div>
        </div>
        <!-- THIRD CARD -->
        <div class="project-card">
          <img src="../../assets/img/projects/discord.png" alt="">
          <div>
            Progetto volto a replicare la grafica del sito della piattaforma Discord.
          </div>
        </div>
        <!-- FOURTH CARD -->
        <div class="project-card">
          <img src="../../assets/img/projects/playstation.png" alt="">
          <div>
            Progetto volto a replicare la grafica del sito di Playstation.
          </div>
        </div>
        <!-- FIFTH CARD -->
        <div class="project-card">
          <img src="../../assets/img/projects/boolzapp.png" alt="">
          <div>
            Progetto il cui obiettivo era quello di replicare il funzionamento di un applicazione stile Whatsapp.
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: 'MyMain',
}
</script>

<style lang="scss">
@import '../../assets/scss/variables.scss';
// MAIN
main{
  width: 60%;
  margin: 0 auto;
}
// TITLES
.titles{
  font-size: 4rem;
  text-align: center;
  margin-top: 100px;
}
// ABOUT SECTION
.about-section{
  text-align: center;
}
.about-title{
  font-size: 4rem;
}
// MAIN IMG
.img{
  margin-top: 100px;
  width: 30%;
  border-radius: 50%;
}
// DISCOVER TEXT
.discover-text{
  margin-top: 100px;
}
i{
  height: 100px;
  width: 100px;
}
// SKILLS SECTION
// CARDS
.skills-cards{
  display: flex;
  justify-content: center;
  margin-top: 100px;
}
.skill-card{
  width: 40%;
  border: 1px solid $semi-white;
  padding: 150px 0;
  text-align: center;
}
.skill-card:first-child{
  border-top-left-radius: 25px;
  border-bottom-left-radius: 25px;
}
.skill-card:last-child{
  border-top-right-radius: 25px;
  border-bottom-right-radius: 25px;
}
.skill-card h2{
  margin-bottom: 3rem;
}
.skill-card ul li{
  margin-top: 10px;
}
.tech-icon{
  border-radius: 50%;
  width: 30%;
  // margin-top: 50px;
  margin-bottom: 10px;
}
// PROJECTS SECTION
.projects-cards{
  margin: 100px 0;
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}
.project-card{
  width: 30%;
  margin: 10px 0;
  padding: 15px 40px;
  border-radius: 25px;
  border: 1px solid $semi-grey;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}
.project-card img{
  width: 80%;
  height: 200px;
  margin: 20px 0;
  border-radius: 10px;
  object-fit: cover;
  border: 1px solid $semi-white;
}
</style>