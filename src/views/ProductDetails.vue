<script setup>
import productsJson from '@/assets/products.json'
</script>
<template>
  <main>
    <h2>Product Details</h2>
    <p>Product ID: {{ $route.params.id }}</p>
    <ul>
      <li>
        <h3>{{ productsJson[$route.params.id - 1].name }}</h3>
        <p>{{ productsJson[$route.params.id - 1].description }}</p>
      </li>
    </ul>
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
</style>
