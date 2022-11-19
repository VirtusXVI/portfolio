<template>
  <main>
    <!-- ABOUT SECTION -->
    <div class="container container-blue">
      <div class="about-adjustments">
        <section id="about-section" class="about-section">
          <div class="my-img">
            <img class="pattern" src="../../assets/img/pattern2.png" alt="">
            <img class="img" src="../../assets/img/me.jpg" alt="">
            <img class="pattern-2" src="../../assets/img/pattern2.png" alt="">
          </div>
          <div class="title-logo">
            <div>
              <div class="about-title-yellow">
                Ciao, sono Manuel.
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
    </div>
    <div class="yellow-background blue-text">
      <div class="container container-yellow">
        <section id="skills-section" class="skills-section">
          <div class="about-title-blue">
            Le Mie Skills
          </div>
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
    <section id="projects-section" class="projects-section">
      <div class="container blue-background">
        <div class="projects-adjustments">
          <div class="about-title-yellow">
            I miei progetti
          </div>
          <SimpleCarousel>
            <div class="slide slide-1">
              <a href="www.google.com">
                <div>
                  BOOLFLIX
                </div>
              </a>
            </div>
            <div class="slide slide-2">
              <a href="www.google.com">
                <div>
                  DELIVEBOO
                </div>
              </a>
            </div>
            <div class="slide slide-3">
              <a href="www.google.com">
                <div>
                  DISCORD
                </div>
              </a>
            </div>
            <div class="slide slide-4">
              <a href="www.google.com">
                <div>
                  PLAYSTATION
                </div>
              </a>
            </div>
          </SimpleCarousel>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import SimpleCarousel from "vue2-simple-carousel";

export default {
  name: 'MyMain',
  components:{
    SimpleCarousel,
  }
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
}
// BACKGROUNDS
.yellow-background{
  background-color: $text-color;
}
.blue-background{
  background-color: $background-color;
  border-left: 2px solid $text-color;
  border-right: 2px solid $text-color;
}
.blue-text{
  color: $background-color;
}
// CONTAINERS
.container-blue{
  border-left: 2px solid $text-color;
  border-right: 2px solid $text-color;
}
.container-yellow{
  border-left: 2px solid $background-color;
  border-right: 2px solid $background-color;
}

// ABOUT SECTION
.about-adjustments{
  display: flex;
  justify-content: center;
}
.about-section{
  width: 90%;
  display: flex;
  justify-content: center;
  // align-items: center;
  padding-top: 100px;
  padding-bottom: 50px;
}
.about-title-yellow{
  font-size: 6rem;
  color: $text-color;
  text-align: center;
}
.about-title-blue{
  font-size: 6rem;
  color: $background-color;
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
.projects-section{
  background-image: url(../../assets/img/pattern2.png);
  background-size: 150px 150px;
}
.projects-adjustments{
  padding: 4rem 0;
}
// CAROUSEL
.carousel-wrapper{
  width: 90%;
  margin: 0 auto;
}
.carousel{
  margin-top: 3rem;
}
.carousel__element{
  height: 300px;
}
.slide{
  height: 300px;
  width: 100%;
  line-height: 300px;
  text-align: center;
  border-radius: 25px;
  margin: 1rem;
}
// SLIDES
.slide span{
  height: 100%;
}
.slide-1{
  background-image: url(../../assets/img/projects/boolflix.png);
}
.slide-2{
  background-image: url(../../assets/img/projects/deliveboo.png);
}
.slide-3{
  background-image: url(../../assets/img/projects/discord.png);
}
.slide-4{
  background-image: url(../../assets/img/projects/playstation.png);
}
.slide-4 a{
  color: $background-color;
}
// BUTTONS
.carousel button{
  background-color: rgba($color: $background-color, $alpha: 0.8);
  border: 1px solid $text-color;
  cursor: pointer;
  height: 100px;
  padding: 0 1rem;
  border-radius: 10px;
  color: $text-color;
  display: block;
}
button:hover {background-color: rgba($color: $text-color, $alpha: 0.7);}

button:active {
  box-shadow: 0 2px #666;
  transform: translateY(4px);
}
</style>