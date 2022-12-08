<template>
  <Navbar />
  <main>
    <p v-if="show" :class="backgroundColor">This is a conditional element</p>
    <button @click="changePColor">Change color</button>
    <Card />
  </main>
  <Footer />
</template>

<script setup>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
import Card from "./components/Card.vue";
import { ref } from "vue";

const show = ref(true);

let backgroundColor = ref("blue");

const changePColor = () => {
  backgroundColor.value === "blue"
    ? (backgroundColor.value = "grey")
    : (backgroundColor.value = "blue");
};
</script>

<style scoped>
.blue {
  background-color: lightblue;
}

.grey {
  background-color: lightgrey;
}
</style>
