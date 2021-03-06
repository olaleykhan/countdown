<template>
  <!-- <HelloWorld msg="Wp"/> -->
  <!-- <Heading headingText="WE'RE LAUNCHING SOON" /> -->
  <Top/>
  <Footer/>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
// import Heading from './components/Heading.vue';
import Top from './components/Top.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld,
    Top,
    Footer,
    // Heading,
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Red+Hat+Text:wght@400&display=swap');
*{
  padding: 0;
  margin: 0;
  /* box-sizing: content-box; */
}

:root{
  --White: hsl(0, 0%, 100%);
--Dark-desaturated-blue: hsl(236, 21%, 26%);
--Very-dark-blue: hsl(235, 16%, 14%);
--black-dark-blue: hsl(234, 17%, 12%);
--grayish-blue: hsl(237, 18%, 59%);
--soft-red: hsl(345, 95%, 68%);
}

#app {
  font-family: 'Red Hat Text', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /* color: #2c3e50; */
  /* margin-top: 60px; */
  background-color: var(--black-dark-blue);
  background-image: url("../src/assets/bg-stars.svg");
  height: 100vh;
  color:var(--White)
}
body{
  
}
</style>
