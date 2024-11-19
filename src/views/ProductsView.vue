<script setup>
import ProductsCmp from '../components/ProductsCmp.vue'
</script>
<template>
  <main>
    <h2>Products</h2>
    <ProductsCmp />
  </main>
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