<template>
  <div id="app">
    <AutocompleteBundledUi />
  </div>
</template>

<script>
import AutocompleteBundledUi from './components/AutocompleteBundledUi.vue'

export default {
  name: 'App',
  components: {
    AutocompleteBundledUi
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
