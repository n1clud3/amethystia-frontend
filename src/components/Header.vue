<script setup>
defineProps(['title', 'subtitle'])
</script>

<template>
  <header>
    <h1>{{ title }}</h1>
    <div class="subtitle">{{ subtitle }}</div>
  </header>
</template>

<style scoped>
header {
  text-align: center;
  padding: 0.5rem;
}

h1 {
  margin: 0;
  padding: 0;
}
.subtitle {
  margin-bottom: 0.5rem;
  padding: 0;
}
</style>