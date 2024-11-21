<script setup>
import { ref } from 'vue'
const query = ref('')
</script>
<template>
  <form :action="`/resultats/query=${query}`">
    <input type="text" v-model="query" />
    <button type="submit">Search</button>
  </form>
</template>
<style scoped>
main {
  display: flex;
  justify-content: center;
  align-items: center;
  height: auto;
  width: 100%;
  flex-direction: column;
}
</style>
