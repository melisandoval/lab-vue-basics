<template>
  <Navbar />
  <main>
    <p v-if="show">This is a conditional element</p>
  </main>
  <Footer />
</template>

<script setup>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
import { ref } from "vue";

const show = ref(true);
</script>

<style scoped></style>
