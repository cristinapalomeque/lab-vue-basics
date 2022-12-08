<template>
  <div class="flex space-x-4 bg-slate-200" v-if="showFooter">
    <a>About us</a>
    <a>Social Media</a>
  </div>
  <button
    class="border-solid border-2 border-amber-600 bg-amber-300 rounded mt-4 px-3"
    @click="showFooter = !showFooter"
  >
    Toggle
  </button>
</template>

<script setup>
import { ref } from "vue";
let showFooter = ref(true);
</script>

<style></style>
