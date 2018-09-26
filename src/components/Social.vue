<template>
  <div>
    <div v-for="site in sites" :key="site.url">
      <div v-if="site.name.toLowerCase() == 'twitter'">
        <img height="32" width="32" src="https://unpkg.com/simple-icons@latest/icons/twitter.svg" />
        <a href={{ site.url}}>
      </div>
      <div v-else-if="site.name.toLowerCase() == 'facebook'">
        <img height="32" width="32" src="https://unpkg.com/simple-icons@latest/icons/facebook.svg" />
        <a href={{ site.url}}>
      </div>
      <div v-else>
        <a href={{ site.url}}>
      </div>

    </div>
  </div>
</template>

<script>
module.exports = {
  props: ["sites"]
};
</script>

<style>
</style>
