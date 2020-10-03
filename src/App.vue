<template>
  <div id="app">
    <div class="columns">
      <div class="column"></div>
      <div class="column">
        <Accordion />
      </div>
      <div class="column"></div>
    </div>
  </div>
</template>

<script>
import Accordion from './components/Accordion.vue';
export default {
  name: 'App',
  components: {
    Accordion
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
