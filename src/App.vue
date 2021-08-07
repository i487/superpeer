<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>
export default {
  name: "App"
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  list-style-type: none;
}

body {
  font-family: 'Roboto', sans-serif;
}
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 15px;
}
</style>
