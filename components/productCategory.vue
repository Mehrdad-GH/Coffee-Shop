<template>
  <div class="mb-96">
    <div class="mx-20 flex justify-between">
      <div class="flex">
        <img src="/icons/coffeeBean.png" alt="" />
        <div class="mr-3">
          <h1 class="text-3xl font-black">دسته بندی محصولات</h1>
          <h2>از میان بهترین ها ، بهترین هارا برای شما فراهم کرده ایم!</h2>
        </div>
      </div>

      <div>
        <FontAwesome
          class="bg-[#F2E5DA] rounded-md p-2 ml-2 swiper-button-next"
          :icon="faCoffee"
        />
        <FontAwesome
          class="bg-[#F2E5DA] rounded-md p-2 swiper-button-prev"
          :icon="faChevronLeft"
        />
      </div>
    </div>

    <div class="text-center">
      <Swiper
      class="mt-10"
        :modules="[SwiperAutoplay, SwiperNavigation]"
        :slides-per-view="9"
        :loop="true"
        :effect="'creative'"
        :autoplay="{
          delay: 8000,
          disableOnInteraction: true,
        }"
        :navigation="{
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev',
        }"
      >
        <SwiperSlide v-for="slide in 10" :key="slide">
          <strong>{{ slide }}</strong>
        </SwiperSlide>
      </Swiper>
    </div>
  </div>
</template>

<script setup>
import { faChevronRight, faChevronLeft } from "@fortawesome/free-solid-svg-icons";
import { faCoffee } from "@fortawesome/free-solid-svg-icons";

const category = [
  {title: "قهوه ساز ها" , icon : ""}
]

</script>

<style scoped>

.swiper-button-next,
.swiper-button-prev {
position: static !important;
color: black !important;
display: inline !important;
width: 15px !important;
height: fit-content !important;
}

</style>
