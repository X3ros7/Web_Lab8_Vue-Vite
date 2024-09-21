<script setup lang="ts">
import { reactive } from "vue";
import { expenses } from "./../../expenses";
import ExpenseItem from "./../ExpenseItem/ExpenseItem.vue";

const items = reactive(expenses);
</script>

<template>
  <div class="expenses">
    <ExpenseItem :items="items" />
  </div>
</template>

<style scoped></style>
