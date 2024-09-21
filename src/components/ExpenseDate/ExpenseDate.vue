<script setup lang="ts">
const props = defineProps<{ date: Date }>();

console.log(props.date);
</script>

<template>
  <div class="date-box">
    <span class="month">{{
      props.date?.toLocaleString("eng", { month: "long" })
    }}</span>
    <span class="year">{{
      props.date?.toLocaleString("eng", { year: "numeric" })
    }}</span>
    <span class="day">{{ props.date?.getDate() }}</span>
  </div>
</template>

<style scoped>
.date-box {
  background-color: #2a2a2a;
  color: white;
  height: 90px;
  width: 90px;
  border: 1.5px solid white;
  border-radius: 7px;
  margin: 15px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
}

.month {
  font-weight: bold;
}

.day {
  font-size: 30px;
}
</style>
