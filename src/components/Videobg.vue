<template>
  <div class="w-full h-84 overflow-hidden relative" id="video_contain">
    <video autoplay muted loop id="myVideo" class="">
      <source :src="popular" class="object-cover" type="video/mp4" />
      Your browser does not support HTML5 video.
    </video>
    <div
      class="w-full h-84 absolute bg-black text-white top-0 right-0 opacity-50 flex items-center justify-center"
    ></div>

    <div
      class="absolute top-0 right-0 h-84 w-full flex flex-col justify-center items-center"
    >
      <!-- image -->
      <div>
        <img src="@/assets/sulov.jpg" alt="" class="h-20 w-20 rounded-full" />
      </div>
      <div class="text-white font-bold text-xl">CEO Sulov Sigdel</div>
      <div class="text-white font-bold text-2xl">Popular Unisex Saloon</div>
    </div>
  </div>
</template>

<script>
import popular from "@/assets/popular.mp4";

export default {
  data() {
    return {
      popular: popular,
    };
  },
};
</script>

<style scoped>
</style>
