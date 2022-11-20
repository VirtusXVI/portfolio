<template>
  <header class="header-container">
    <!-- BURGER -->
    <div class="burger" @click="changeBurgerStatus()">
      <i class="fa-solid fa-bars"></i>
    </div>
    <!-- BURGER MENU-->
    <div :class="this.visible_burger ? 'burger-menu-1' : 'burger-menu'">
      <ul>
        <li @click="changeBurgerStatus()"><i class="fa-solid fa-bars"></i></li>
        <li @click="changeBurgerStatus()"><a href="#about-section">ABOUT</a></li>
        <li @click="changeBurgerStatus()"><a href="#skills-section">SKILLS</a></li>
        <li @click="changeBurgerStatus()"><a href="#projects-section">PROGETTI</a></li>
        <li @click="changeBurgerStatus()"><a href="#contacts-section">CONTATTI</a></li>
      </ul>
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
  data() {
    return{
      visible_burger: false,
    }
  },
  methods:{
    changeBurgerStatus(){
      this.visible_burger = !this.visible_burger;
    }
  }
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
// BURGER
.burger{
  padding: 2rem 2rem;
  display: none;
  justify-content: center;
}
// BURGER MENU
.burger-menu{
  display: none;
  position: absolute;
  height: 100vh;
  width: 100%;
  background-color: $background-color;
}
.burger-menu-1{
  display: block;
  position: absolute;
  height: 100vh;
  width: 100%;
  background-color: $background-color;
}
.burger-menu-1 ul{
  height: 50%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-evenly;
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
  nav ul li{
    margin: 2rem 8px;
  }
  nav{
    display: none;
  }
  .burger{
    display: flex;
  }
}
</style>