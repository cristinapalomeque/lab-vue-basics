<template>
  <Navbar></Navbar>

  <p>Iteration 1</p>
  <div>Math operation {{ 2 + 2 }}</div>

  <p>Iteration 2</p>
  >
  <div>{{ operation(2, 3) }}</div>

  <p>Iteration 4</p>
  <Posts></Posts>
  <p>Iteration 3</p>
  <Footer></Footer>
</template>

<script setup>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
import Posts from "./components/Posts.vue";
function operation(a, b) {
  return a + b;
}
</script>

<style></style>
