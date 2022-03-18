<script setup>
defineProps(['currentLocation', 'homeButtonAction', 'apiButtonAction']);
</script>

<template>
  <nav>
    <span class="buttons">
      <button @click="homeButtonAction">Home</button>
      <button @click="apiButtonAction">API</button>
    </span>
    <span class="current_location">You are currently at <b>{{ currentLocation }}</b></span>
  </nav>
</template>

<style>
nav {
  background-color: rgb(255, 244, 253);
  padding: 1rem;
  margin-bottom: 1rem;
}

.buttons {
  padding: 0.5rem;
}

.current_location {
  margin: 0.5rem;
}

button {
  padding: 0.5rem;
  background-color: rgb(255, 221, 252);
  border: none;
  font-family: 'Source Sans Pro', sans-serif;
  font-size: 18px;
  transition: all 150ms ease-in-out;
}

button:hover {
  background: rgb(255, 127, 202);
}
</style>