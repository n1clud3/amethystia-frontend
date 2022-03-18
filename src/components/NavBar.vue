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

<style lang="scss">
nav {
  background-color: whitesmoke;
  padding: 1em;
  margin-bottom: 1rem;

  .buttons {
    transition: 150ms ease;
    :hover {
      background-color: aquamarine;
    }

    button {
      padding: 0.5rem;
      background-color: rgb(219, 219, 219);
      border: none;
      font-size: 16px;
    }
  }

  .current_location {
    margin: 0.5rem;
  }
}
</style>