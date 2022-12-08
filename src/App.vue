<template>
  <Navbar></Navbar>

  <p>Iteration 1</p>
  <div>Math operation {{ 2 + 2 }}</div>

  <p>Iteration 2</p>
  >
  <div>{{ operation(2, 3) }}</div>

  <p>Iteration 4</p>
  <Posts></Posts>

  <p>Iteration 5</p>
  <div :class="{ blue: changeColor }">I am learning Vue</div>
  <button @click="changeColor = !changeColor">Toggle</button>

  <p>Iteration 3</p>
  <Footer></Footer>
</template>

<script setup>
import { ref } from "vue";
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
import Posts from "./components/Posts.vue";
function operation(a, b) {
  return a + b;
}

let changeColor = ref(true);
</script>

<style>
.blue {
  background-color: blue;
  color: white;
  width: 30rem;
  border: solid 1px black;
}
</style>
