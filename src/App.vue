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

#app {
  position: absolute;
  width: 100%;
  // background-image: url('./assets/img/background.jpg');
  // background-repeat: no-repeat;
  // background-size: contain;
}
</style>
