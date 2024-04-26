<template>
  <canvas id="can1"></canvas>
  <canvas id="can2"></canvas>
</template>
<script setup>
import { onMounted } from "vue";
import { createTextImage } from "@sunny-117/text-image";
onMounted(() => {
  createTextImage({
    canvas: document.querySelector("#can1"),
    replaceText: "6",
    source: {
      video: "../public/1.mp4",
    },
  });
});
</script>
