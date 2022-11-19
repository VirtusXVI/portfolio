<template>
  <header class="header-container">
    <!-- LOGO -->
    <div>
      <div>
        <!-- <a href="#">Aveta Manuel</a> -->
      </div>
    </div>
    <!-- NAV -->
    <nav>
      <ul>
        <li><a href="#about-section">ABOUT</a></li>
        <li><a href="#skills-section">SKILLS</a></li>
        <li><a href="#projects-section">PROGETTI</a></li>
        <li><a href="#contacts-section">CONTATTI</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'MyHeader',
}
</script>

<style lang="scss">
@import '../../assets/scss/common.scss';
.header-container{
  width: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  position: fixed;
  z-index: 999;
  background-color: $background-color;
}
// NAV
nav ul{
  display: flex;
  align-items: center;
  height: 100%;
}
nav ul li{
  margin: 2rem 2rem;
}
// MEDIA QUERIES
@media only screen and (max-width: 1270px) {
  nav{
    display: none;
  }
}
</style>