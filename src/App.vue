<template>
  <to_do />
</template>

<script>
import to_do from './components/to_do.vue'

export default {
  name: 'App',
  components: {
    to_do
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
