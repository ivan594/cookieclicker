<template>
  <div id="app">
    <Clicker 
      title="CookieClicker"
    />
  </div>
</template>

<script>
import Clicker from './components/Clicker.vue'

export default {
  name: 'App',
  components: {
    Clicker,
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
