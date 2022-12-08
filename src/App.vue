<template>
  <Navbar></Navbar>

  <p class="font-bold">Iteration 1</p>
  <div>Math operation: 2+2= {{ 2 + 2 }}</div>

  <p class="font-bold">Iteration 2</p>
  >
  <div>{{ operation(2, 3) }}</div>

  <p class="font-bold">Iteration 4</p>
  <Posts></Posts>

  <p class="font-bold">Iteration 5</p>
  <div :class="{ orange: changeColor }">I am learning Vue</div>
  <button
    class="border-solid border-2 border-amber-600 rounded mt-4 px-3 bg-amber-300"
    @click="changeColor = !changeColor"
  >
    Toggle
  </button>

  <p class="font-bold">Iteration 3</p>
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
.orange {
  background-color: orangered;
  color: white;
  width: 30rem;
  border: solid 1px black;
}
</style>
