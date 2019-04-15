<template>
  <div id="app" class="app">
    <Home />
    <hr />
    <Results />
  </div>
</template>

<script>
import Home from './components/Home.vue';
import Results from './components/Results.vue';

export default {
  name: 'app',
  components: {
    Home,
    Results,
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
}
</style>
