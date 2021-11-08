<template>
  <div>
    <img alt="Noisy birds" src="../assets/birds.svg" width="100" />
    <h1>Twitter Follow Stats</h1>
    <p>Cut the noise so you can appreciate the signal.</p>
    <p>
      Shows you whose tweets are clogging your timeline. Does
      <strong>not</strong> unfollow anybody automatically.
    </p>
    <div>
      <strong>Analyze your follow list:</strong>
      <button>Sign in with Twitter</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AppHome',
};
</script>

<style lang="scss" scoped>
img {
  max-width: 500px;
  width: 33vw;
}
</style>
