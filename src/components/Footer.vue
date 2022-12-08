<template>
  <div v-if="showFooter">
    <a>About us</a>
    <a>Social Media</a>
  </div>
</template>

<script setup>
import { ref } from "vue";
let showFooter = ref(true);
</script>

<style></style>
