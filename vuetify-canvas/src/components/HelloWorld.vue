<template>
  <canvas id="tutorial" width="800" height="600"></canvas>
</template>

<script lang="ts" setup>
import { onMounted } from 'vue';

onMounted(() => {
  const canvas = document.getElementById("tutorial");
  if (canvas instanceof HTMLCanvasElement) {
    const ctx = canvas.getContext("2d");
    if (ctx) {
      ctx.fillStyle = "green";
      ctx.fillRect(20, 10, 150, 100);
    }

  }

})
</script>
<style scoped>
canvas {
  border: 1px solid black;
}
</style>
