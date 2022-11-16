<template>
  <main>
    <section class="about-section">
      <div class="about-title">
        Ciao, sono Manuel. Sono un Full-Stack web developer
      </div>
      <div>
        <img class="img" src='../../assets/img/me.jpg' alt="me">
      </div>
      <div class="discover-text">
        <a href="#">
          Scopri cosa so fare
        </a>
      </div>
    </section>
    <section class="projects-section">

    </section>
    <section class="skills-section">

    </section>
  </main>
</template>

<script>
export default {
  name: 'MyMain',
}
</script>

<style lang="scss">
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
</style>