<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';

import {ref} from 'vue';

const navCurrentLocation = ref("the front page of Amethystia");

const navHomeButtonAction = (() => {
  console.log('clicked home button')
})

const navApiButtonAction = (() => {
  console.log('clicked api button')
})
</script>

<template>
  <NavBar 
    :currentLocation="navCurrentLocation"
    :homeButtonAction="navHomeButtonAction"
    :apiButtonAction="navApiButtonAction"
  />
  <main>
    Lorem ipsum dolor sit amet consectetur adipisicing elit.
    Beatae quidem facilis fuga ipsum adipisci, eum accusamus minus illo!
    Accusamus dolore alias ex ab, iure unde nihil facilis in incidunt saepe?
  </main>
  <Footer/>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro&display=swap');

body {
  margin: 0;
}

#app {
  font-family: 'Source Sans Pro', sans-serif;
  font-size: 18px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

main {
  margin-left: auto;
  margin-right: auto;
  max-width: 50rem;
  //padding: 1rem;
}
</style>
