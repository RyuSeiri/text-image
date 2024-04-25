<template>
  <canvas></canvas>
</template>

<script setup>
import { createTextImage } from '@sunny-117/text-image';
import {onMounted} from 'vue';

onMounted(() => {
  createTextImage({
    canvas: document.querySelector('canvas'),
    source: {
      text: 'Text Image',
    },
  });
})
</script>

<style scoped>
.titleBox {
  background-color: blueviolet;
}
</style>