<template>
  <div v-if="showFooter">
    <a>About us</a>
    <a>Social Media</a>
  </div>
  <button @click="showFooter = !showFooter">Toggle</button>
</template>

<script>
// import { ref } from "vue";
// let showFooter = ref(true);
export default {
  data() {
    return {
      showFooter: true,
    };
  },
};
</script>

<style></style>
