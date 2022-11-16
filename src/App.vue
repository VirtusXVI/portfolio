<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/> -->
    <MyHeader/>
    <MyMain/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
// import HelloWorld from './components/HelloWorld.vue';
import MyHeader from './components/main-components/MyHeader.vue';
import MyMain from './components/main-components/MyMain.vue';

@Component({
  components: {
    // HelloWorld,
    MyHeader,
    MyMain
  },
})
export default class App extends Vue {}
</script>

<style lang="scss">
@import './assets/scss/common.scss';

// #app {
//   font-family: Avenir, Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
//   margin-top: 60px;
// }
</style>
