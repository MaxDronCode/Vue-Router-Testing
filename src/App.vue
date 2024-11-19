<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <nav>
      <ul>
        <li>
          <RouterLink to="/">Home</RouterLink>
        </li>
        <li>
          <RouterLink to="/about">About</RouterLink>
        </li>
        <li>
          <RouterLink to="/contact">Contact</RouterLink>
        </li>
        <li>
          <RouterLink to="/products">Products</RouterLink>
        </li>
      </ul>
    </nav>
  </header>
  <RouterView />
</template>

<style scoped>
* {
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}
nav {
  background-color: #333;
  color: white;
  display: flex;
  justify-content: space-around;
  border-radius: 0 0 5px 5px;
}
a {
  color: white;
}
ul {
  display: flex;
  list-style-type: none;
  padding: 0;
  width: 100%;
  justify-content: space-around;
}
</style>
