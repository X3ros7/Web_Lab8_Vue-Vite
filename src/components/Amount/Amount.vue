<script setup lang="ts">
const props = defineProps<{ amount: number }>();
</script>

<template>
  <div class="amount">${{ props.amount }}</div>
</template>

<style scoped>
.amount {
  color: white;
  background-color: #40005d;
  width: 120px;
  height: 30px;
  padding: 5px 10px;
  border: 1.5px solid white;
  border-radius: 5px;
  display: flex;
  flex-direction: column;
  align-items: center;
  font-size: 22.5px;
  font-weight: bold;
  margin-right: 10px;
}
</style>
