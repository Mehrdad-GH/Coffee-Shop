<template>
  <div>
    <HeroSection />
    <img class="relative my-16 z-10" src="/icons/Separator.png" alt="" />
    <img
      class="absolute top-72 mt-10 left-0 opacity-5 z-0"
      src="/icons/vector.png"
      alt=""
    />
    <productCategory />
  </div>
</template>

<script setup>
import productCategory from "~/components/productCategory.vue";
</script>

<style scoped></style>
