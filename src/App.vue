<template>
  <div id="app" class="app">
    <img alt="Noisy birds" src="./assets/birds.svg" width="100" />
    <HelloWorld msg="Twitter Follow Stats" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'app',
  components: {
    HelloWorld,
  },
};
</script>

<style lang="scss">
$color-text-default: #2c3e50;

.app {
  color: $color-text-default;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin-top: 60px;
  text-align: center;

  img {
    max-width: 500px;
    width: 33vw;
  }
}
</style>
