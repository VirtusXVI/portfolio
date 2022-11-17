<template>
  <main>
    <!-- ABOUT SECTION -->
    <section class="about-section">
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
    <section class="skills-section">
      <div class="projects-title">
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
    <section class="projects-section">
      <div class="projects-title">
        I MIEI PROGETTI
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
  border: 1px solid $semi-grey;
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
.projects-title{
  font-size: 4rem;
  text-align: center;
  margin-top: 100px;
}
</style>