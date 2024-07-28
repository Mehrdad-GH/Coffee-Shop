<template>
  <div class="flex text-white mx-20 mt-10 h-[60vh]">
    <div
      class="flex flex-col justify-center pr-16 h-full w-[30%] bg-[#28221E] rounded-xl py-10"
    >
      <img class="w-fit" src="/icons/fantesyLogo.png" alt="" />

      <div class="flex mt-7">
        <h1 class="font-black text-6xl relative z-10">اریک کافه</h1>
        <img class="h-fit translate-x-3 z-0" src="/icons/leaf.png" alt="" />
      </div>

      <h2 class="font-thin mt-4 opacity-50">
        کامل ترین تجهیزات کافه و رستوران در ایران
      </h2>

      <button
        class="flex gap-3 w-fit px-3 py-2 rounded-full items-center mt-10 bg-white/20 duration-300 hover:bg-[#9E624C]"
      >
        مشاهده محصولات <FontAwesome :icon="faArrowLeft" />
      </button>
    </div>

    <div
      class="flex relative z-10 bg-gradient-to-r from-[#E8DFD6] from-45% to-[#847669] h-full w-[70%] mr-7 rounded-xl"
    >
      <div class="flex flex-row-reverse">
        <div class="flex justify-end items-end h-full  w-1/2">
          <img class="d" src="/icons/slideBack.png" alt="" />
        </div>
        <div
          class="flex flex-col w-1/2 gap-5 justify-center items-start mr-10 text-white "
        >
          <h1 class="text-6xl font-black">کافــــــه از تـــــــــو</h1>
          <h2 class="opacity-80">تجهیزات با ما</h2>
          <FontAwesome :icon="faArrowLeft" />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { faArrowLeft } from "@fortawesome/free-solid-svg-icons";
</script>

<style></style>
