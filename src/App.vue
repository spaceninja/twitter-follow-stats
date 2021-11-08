<template>
  <AppHome />
  <hr />
  <AppResults />
</template>

<script>
import AppHome from './components/AppHome.vue';
import AppResults from './components/AppResults.vue';

export default {
  components: {
    AppHome,
    AppResults,
  },
};
</script>
