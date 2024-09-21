<script setup lang="ts">
import ExpenseDate from "../ExpenseDate/ExpenseDate.vue";
import Amount from "../Amount/Amount.vue";

defineProps<{
  items: import("/home/ubuntu/src/others/first-vue-project/node_modules/vue/dist/vue").Reactive<
    import("./../../expenses").expense[]
  >;
}>();
</script>

<template>
  <div class="expense" v-for="item in items">
    <ExpenseDate :date="item.date" />
    <div class="item">{{ item.title }}</div>
    <Amount :amount="item.amount" />
  </div>
</template>

<style scoped>
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
