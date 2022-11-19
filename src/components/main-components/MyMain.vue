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
              <div class="about-title-yellow about-intro">
                Ciao, <br> sono Manuel.
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
      <div class="container blue-background no-borders">
        <div class="projects-adjustments">
          <div class="about-title-yellow">
            I miei progetti
          </div>
          <SimpleCarousel>
            <div class="slide slide-1">
              <a href="https://github.com/VirtusXVI/vue-boolflix">
                <div>
                  BOOLFLIX
                </div>
              </a>
            </div>
            <div class="slide slide-2">
              <a href="https://github.com/VirtusXVI/deliverboo">
                <div>
                  DELIVEBOO
                </div>
              </a>
            </div>
            <div class="slide slide-3">
              <a href="https://github.com/VirtusXVI/htmlcss-discord">
                <div>
                  DISCORD
                </div>
              </a>
            </div>
            <div class="slide slide-4">
              <a href="https://github.com/VirtusXVI/htmlcss-playstation">
                <div>
                  PLAYSTATION
                </div>
              </a>
            </div>
          </SimpleCarousel>
        </div>
      </div>
    </section>
    <div class="yellow-background blue-text">
      <div class="container container-yellow">
        <section id="contacts-section" class="contacts-section">
          <ul>
            <li><a href="https://www.linkedin.com/in/manuel-aveta/"><i class="fa-brands fa-linkedin-in"></i></a></li>
            <li><a href="https://github.com/VirtusXVI"><i class="fa-brands fa-github"></i></a></li>
            <li><a href="mailto:manuel.aveta2001@gmail.com"><i class="fa-solid fa-envelope"></i></a></li>
          </ul>
        </section>
      </div>
    </div>
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
.no-borders{
  border: none;
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
  font-size: 5rem;
  color: $text-color;
  text-align: center;
}
.about-title-blue{
  font-size: 6rem;
  color: $background-color;
}
.about-intro{
  text-align: left;
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
  background-image: url(../../assets/img/pattern.png);
  background-position: center;
  background-size: 245px;
}
.projects-adjustments{
  padding: 4rem 0;
  padding-bottom: 6.5rem;
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
  width: 300px;
  line-height: 300px;
  text-align: center;
  border-radius: 25px;
  margin: 1rem;
  background-position: center top;
}
// SLIDES
.slide span{
  height: 100%;
}
.slide a div{
  background-color: rgba($color: #000000, $alpha: 0.5);
  border-radius: 25px;
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
// BUTTONS
.carousel button{
  background-color: rgba($color: $text-color, $alpha: 0.8);
  border: 1px solid $background-color;
  cursor: pointer;
  height: 50px;
  width: 50px;
  padding: 0 1rem;
  border-radius: 50%;
  color: $background-color;
  display: block;
}
button:hover {background-color: rgba($color: $text-color, $alpha: 0.7);}

button:active {
  box-shadow: 0 2px rgb(0, 0, 0);
  transform: translateY(4px);
}
// CONTACTS SECTION
.contacts-section{
  padding: 1rem 0;
  width: 30%;
  margin: 0 auto;
}
.contacts-section ul{
  display: flex;
  justify-content: space-evenly;
}
.contacts-section ul li a{
  color: $background-color;
  font-size: 2.5rem;
}
// MEDIA QUERIES
@media only screen and (max-width: 1270px) {
  .about-section{
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .my-img{
    width: 80%;
    margin-bottom: 4rem;
  }
  .img{
    width: 100%;
  }
  .pattern{
    width: 40%;
  }
  .pattern-2{
    width: 80%;
  }
  .title-logo{
    width: 80%;
  }
  // .skill-card{
  //   justify-content: center;
  // }
  // .skill-card-2{
  //   justify-content: center;
  // }
}
</style>