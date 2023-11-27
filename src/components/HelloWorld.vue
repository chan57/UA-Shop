<script setup>
import { reactive, ref, onUnmounted } from "vue";

defineProps({
  msg: String,
});
</script>

<template>
  <div>
    <div class="flex justify-center text-2xl font-serif">
      <a class="z-10 text-fuchsia-50 px-10 hover:text-yellow-300 hover:bg-blue-800" href="#"><h3>Home</h3></a>
      <a class="z-10 text-fuchsia-50 px-10  hover:text-yellow-300 hover:bg-blue-800" href="#"><h3>Catalog</h3></a>
      <a class="z-10 text-fuchsia-50 px-10  hover:text-yellow-300 hover:bg-blue-800" href="#"><h3>About</h3></a>
      <a class="z-10 text-fuchsia-50 px-10  hover:text-yellow-300 hover:bg-blue-800" href="#"><h3>Korzina</h3></a>
      <video
        class="absolute z-1 blur-sm "
        style="background-video"
        height="300"
        width="1000"
        autoplay
        loop
        muted
      >
        <source src="/src/assets/zelia11.mp4" type="video/mp4" />
      </video>
    </div>
  </div>
</template>

<style scoped>
</style>
