<script setup lang="ts">
import Expenses from "./../Expenses/Expenses.vue";
</script>

<template>
  <div class="card">
    <Expenses />
  </div>
</template>

<style scoped>
.card {
  background-color: #c0c0c0;
  width: 886px;
  height: 556px;
  border-radius: 0.6rem;
  margin-top: 10px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: stretch;
  padding: 20px;
}

.expense {
  display: flex;
  align-items: center;
  background-color: #4b4b4b;
  border-radius: 0.6rem;
  margin-top: 10px;
  margin-left: 10px;
  margin-right: 10px;
}

.item {
  color: white;
  flex-basis: 600px;
  font-size: 20px;
  font-weight: bold;
}
</style>
