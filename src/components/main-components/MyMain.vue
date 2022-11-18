<template>
  <main>
    <!-- ABOUT SECTION -->
    <div class="container container-blue">
      <section id="about-section" class="about-section">
        <div class="my-img">
          <img class="pattern" src="../../assets/img/pattern2.png" alt="">
          <img class="img" src="../../assets/img/me.jpg" alt="">
          <img class="pattern-2" src="../../assets/img/pattern2.png" alt="">
        </div>
        <div class="title-logo">
          <div>
            <div class="about-title">
              Ciao, sono Manuel. <br>
            </div>
            <div class="about-text">
              Sono un Full-Stack Web Developer.
            </div>
          </div>
          <div class="about-logo">
            <img class="logo" src="../../assets/img/logo.png" alt="">
          </div>
        </div>
      </section>
    </div>
    <div class="yellow-background blue-text">
      <div class="container container-yellow">
        <section id="skills-section" class="skills-section">
          <div class="skill-card">
            <!-- FIRST CARD -->
            <div class="card-img">
              <img src="../../assets/img/frontend.jpg" alt="">
            </div>
            <div class="skill-text-1">
              <div class="titles">
                <h2>FRONT-END DEVELOPMENT</h2>
              </div>
              <ul>
                <li>HTML 5</li>
                <li>CSS 3</li>
                <li>Javascript</li>
                <li>Vue.js</li>
              </ul>
            </div>
          </div>
          <!-- SECOND CARD -->
          <div class="skill-card-2">
            <div class="skill-text-2">
              <div class="titles">
                <h2>BACK-END DEVELOPMENT</h2>
              </div>
              <ul>
                <li>PHP</li>
                <li>Laravel</li>
                
              </ul>
            </div>
            <div class="card-img">
              <img src="../../assets/img/backend.jpg" alt="">
            </div>
          </div>
          <!-- THIRD CARD -->
          <div class="skill-card">
            <div class="card-img">
              <img src="../../assets/img/tools.jpg" alt="">
            </div>
            <div class="skill-text-1">
              <div class="titles">
                <h2>DEV TOOLS</h2>
              </div>
              <ul>
                <li>VS Code</li>
                <li>Git</li>
                <li>GitHub</li>
              </ul>
            </div>
          </div>
        </section>
      </div>
    </div>
    <!-- PROJECTS SECTION -->
    <!-- <section id="projects-section" class="projects-section">
      <div class="titles">
        I MIEI PROGETTI
      </div>
      <div class="projects-cards">
        <div class="project-card">
          <img src="../../assets/img/projects/boolflix.png" alt="">
          <div>
            Progetto riguardante l'utilizzo di API per ricevere dati da un database e mostrarli in pagina.
          </div>
        </div>
        <div class="project-card">
          <img src="../../assets/img/projects/deliveboo.png" alt="">
          <div>
            Progetto di gruppo il cui obiettivo era quello di riprodurre un sistema simile a quello di Deliveroo gestendo i ristoranti,gli ordini e i pagamenti.
          </div>
        </div>
        <div class="project-card">
          <img src="../../assets/img/projects/discord.png" alt="">
          <div>
            Progetto volto a replicare la grafica del sito della piattaforma Discord.
          </div>
        </div>
        <div class="project-card">
          <img src="../../assets/img/projects/playstation.png" alt="">
          <div>
            Progetto volto a replicare la grafica del sito di Playstation.
          </div>
        </div>
        <div class="project-card">
          <img src="../../assets/img/projects/boolzapp.png" alt="">
          <div>
            Progetto il cui obiettivo era quello di replicare il funzionamento di un applicazione stile Whatsapp.
          </div>
        </div>
      </div>
    </section> -->
  </main>
</template>

<script>
export default {
  name: 'MyMain',
}
</script>

<style lang="scss">
@import '../../assets/scss/variables.scss';
// COMMON
// TITLES
.titles h2{
  font-size: 2.2rem;
  color: $background-color;
}

// MAIN
.container{
  width: 90%;
  margin: 0 auto;
  display: flex;
  justify-content: center;
}
.yellow-background{
  background-color: $text-color;
}
.blue-text{
  color: $background-color;
}
.container-blue{
  border-left: 2px solid $text-color;
  border-right: 2px solid $text-color;
}
.container-yellow{
  border-left: 2px solid $background-color;
  border-right: 2px solid $background-color;
}

// ABOUT SECTION
.about-section{
  width: 90%;
  display: flex;
  justify-content: center;
  // align-items: center;
  padding-top: 100px;
  padding-bottom: 50px;
}
.about-title{
  font-size: 6rem;
  color: $text-color;
}
.about-text{
  font-size: 2rem;
}
.title-logo{
  display: flex;
  flex-direction: column;
  width: 40%;
}
.about-logo{
  padding-top: 8rem;
  width: 100%;
  display: flex;
  justify-content: flex-end;
}
.logo{
  width: 50%;
}
// MAIN IMG
.my-img{
  width: 40%;
  position: relative;
}
.img{
  width: 400px;
  border-radius: 50%;
}
// PATTERN
.pattern{
  width: 200px;
  border-radius: 50%;
  position: absolute;
  top: -30px;
  left: -30px;
}
.pattern-2{
  width: 250px;
  border-radius: 50%;
  position: absolute;
  top: 45%;
  left: 35%;
  z-index: -1;
}
// SKILLS SECTION
.skills-section{
  padding: 100px 0;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.skill-card{
  width: 70%;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  margin-top: 2rem;
}
.skill-card-2{
  width: 70%;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  margin-top: 2rem;
}
.card-img{
  width: 15%;
}
.card-img img{
  border-radius: 50%;
}
.skill-text-1{
  width: 50%;
  font-size: 1.2rem;
  text-align: left;
  padding-left: 2.5rem;
}
.skill-text-2{
  width: 50%;
  font-size: 1.2rem;
  text-align: right;
  padding-right: 2.5rem;
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
  border: 1px solid $text-color;
}
</style>