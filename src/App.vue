<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import MyHeader from './components/main-components/MyHeader.vue';
import MyMain from './components/main-components/MyMain.vue';

@Component({
  components: {
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
  min-width: 360px;
}
</style>
