<script setup>
import productsJson from '@/assets/products.json'

</script>
<template>
  <ul>
    <li v-for="product in productsJson" :key="product.id">
      <RouterLink :to="`/products/${product.id}`">{{ product.name }}</RouterLink>
      <p>{{ product.description }}</p>
    </li>
  </ul>
</template>
<style scoped>
p {
  animation: fadeIn 1s ease-in;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}
li {
  animation: slideIn 0.5s ease-in;
}

@keyframes slideIn {
  0% {
    opacity: 0;
    transform: translateX(-20px);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}
</style>