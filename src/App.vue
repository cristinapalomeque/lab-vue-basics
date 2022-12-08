<template>
  <Navbar></Navbar>
  //Iteration 1
  <div>Math operation {{ 2 + 2 }}</div>

  //Iteration 2
  <div>{{ operation(2, 3) }}</div>

  <h1 v-if="awesome">Vue is awesome!</h1>
  <Footer></Footer>
</template>

<script setup>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";

function operation(a, b) {
  return a + b;
}
</script>

<style></style>
