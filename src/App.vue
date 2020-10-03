<template>
  <body
    class="flex flex-col bg-gray-100 w-screen font-header h-screen overflow-hidden"
  >
    <nav class="w-full flex py-4 h-12 items-center bg-red-600">
      <!-- logo part -->
      <div class="w-64 flex justify-center">Popular Unisex</div>
      <div class="flex-1 flex justify-end">
        <ul class="list-none flex mr-10">
          <li class="ml-3">Home</li>
          <li class="ml-3">About Us</li>
          <li class="ml-3">Services</li>
          <li class="ml-3">Galary</li>
          <li class="ml-3">Contact Us</li>
        </ul>
      </div>
    </nav>
    <main class="w-full h-full flex-col overflow-auto flex">
      <!--video bg-->
      <div class="w-full flex justify-center">
        <Videobg />
      </div>
      <div class="w-full">
        <Services />
      </div>
    </main>
  </body>
</template>

<script>
import Videobg from "./components/Videobg";
import Services from "./components/Services";
export default {
  name: "App",
  components: {
    Videobg,
    Services,
  },
};
</script>

<style>
* {
  scroll-behavior: smooth;
}
</style>
