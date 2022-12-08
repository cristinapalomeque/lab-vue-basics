<template>
  <div v-for="item in posts">
    <div>{{ item.title }}</div>
    <div>{{ item.description }}</div>
    <div>{{ item.content }}</div>
  </div>
</template>

<script setup>
import { ref } from "vue";
let posts = ref([
  {
    title: "Brewdog",
    description: "Scottish beer",
    content: "Punk IPA is a fresh and bitter beer",
  },
  {
    title: "Montseny",
    description: "Catalan beer",
    content: "Neipa beer is a fruity beer",
  },
  {
    title: "XXX",
    description: "Australian beer",
    content: "Nice smooth lager",
  },
]);
console.log(posts);
</script>

<style></style>
