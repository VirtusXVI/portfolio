<template>
  <header class="header-container">
    <!-- LOGO -->
    <div class="logo">
      <div>
        <a href="#">Aveta Manuel</a>
      </div>
    </div>
    <!-- NAV -->
    <nav>
      <ul>
        <li><a href="#">HOME</a></li>
        <li><a href="#">ABOUT</a></li>
        <li><a href="#">PROJECTS</a></li>
        <li><a href="#">SKILLS</a></li>
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
  width: 70%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}
// LOGO
.logo{
  font-family: 'Dancing Script', cursive;
  font-size: 2rem;
  width: 30%;
  margin: 1rem 0;
}
// NAV
nav ul{
  display: flex;
  align-items: center;
  height: 100%;
}
nav ul li{
  margin-left: 4rem;
}
</style>