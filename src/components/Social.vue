<template>
  <div>
    <div v-for="site in sites" :key="site.url">
      {{ site.name }}: {{ site.url}}
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
