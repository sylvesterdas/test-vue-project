<template>
  <div @click="onClick">{{ counter }}</div>
</template>

<script setup>
import { defineProps } from "vue";

defineProps(["counter"]);

function onClick() {
  console.log("new test ");
}
</script>

<style scoped>
div {
  padding: 12px;
  font-weight: 500;
  font-size: xx-large;
}
</style>
