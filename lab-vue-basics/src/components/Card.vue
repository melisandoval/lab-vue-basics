<template>
  <div v-for="{ title, descrition, content } in data">
    <h2>{{ title }}</h2>
    <p>{{ descrition }}</p>
    <p>{{ content }}</p>
  </div>
</template>

<script setup>
import { ref } from "vue";

const data = ref([
  {
    title: "Title 1",
    descrition: "This is a subtitle",
    content:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras facilisis in libero nec tincidunt. Suspendisse sed ante augue. Phasellus volutpat eu velit id elementum. Maecenas sed massa tempor, tempor sapien a, pretium neque. Morbi ut massa purus. Sed sed ante sed tellus consectetur tristique. Aliquam erat volutpat. Integer ut finibus urna. Integer vel massa porttitor, mattis libero id, aliquet nulla.",
  },
  {
    title: "Title 2",
    descrition: "This is a subtitle",
    content:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras facilisis in libero nec tincidunt. Suspendisse sed ante augue. Phasellus volutpat eu velit id elementum. Maecenas sed massa tempor, tempor sapien a, pretium neque. Morbi ut massa purus. Sed sed ante sed tellus consectetur tristique. Aliquam erat volutpat. Integer ut finibus urna. Integer vel massa porttitor, mattis libero id, aliquet nulla.",
  },
  {
    title: "Title 3",
    descrition: "This is a subtitle",
    content:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras facilisis in libero nec tincidunt. Suspendisse sed ante augue. Phasellus volutpat eu velit id elementum. Maecenas sed massa tempor, tempor sapien a, pretium neque. Morbi ut massa purus. Sed sed ante sed tellus consectetur tristique. Aliquam erat volutpat. Integer ut finibus urna. Integer vel massa porttitor, mattis libero id, aliquet nulla.",
  },
]);
</script>
