<template>
  <div id="app">
    <div class="columns">
      <div class="column"></div>
      <div class="column">
        <Accordion />
        <L2 />
        <L3 />
      </div>
      <div class="column"></div>
    </div>
  </div>
</template>

<script>
import Accordion from './components/Accordion.vue';
import L2 from './components/L2.vue';
import L3 from './components/L3.vue';

export default {
  name: 'App',
  components: {
    Accordion,
    L2,
    L3
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
