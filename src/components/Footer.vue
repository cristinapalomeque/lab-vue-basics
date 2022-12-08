<template>
  <div v-if="showFooter">
    <a>About us</a>
    <a>Social Media</a>
  </div>
  <button @click="showFooter = !showFooter">Toggle</button>
</template>

<script setup>
import { ref } from "vue";
let showFooter = ref(true);
</script>

<style></style>
