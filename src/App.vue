<template>
  <!-- <HelloWorld msg="Wp"/> -->
  <heading headingText="WE'RE LAUNCHING SOON" />
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
import Heading from './components/Heading.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld,
    Heading,
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
