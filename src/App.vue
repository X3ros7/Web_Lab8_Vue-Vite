<script setup lang="ts">
import Card from "./components/Card/Card.vue";
</script>

<template>
  <h1>My Expenses Template</h1>
  <div class="container">
    <Card />
  </div>
</template>

<style scoped>
.container {
  display: flex;
  justify-content: center;
}
</style>
