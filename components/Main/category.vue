<template>
  <div class="mt-7">
    <div class="flex flex-col gap-4 md:flex-row md:justify-between md:items-center mx-4 sm:mx-8 md:mx-16">
      <div class="flex items-center gap-4">
        <UIcon
          size="40"
          class="text-Primary"
          name="streamline:coffee-bean-solid"
        />
        <div class="flex flex-col">
          <h1 class="font-semibold text-xl">دسته بندی محصولات</h1>
          <h2 class="font-normal">
            از میان بهترین ها ، بهترین هارا برای شما فراهم کرده ایم!
          </h2>
        </div>
      </div>

      <div class="flex gap-2">
        <div @click="goPrevSlide" class="bg-[#F2E5DA] rounded-xl pt-2 px-1 ">
          <UIcon size="28" name="material-symbols:arrow-forward-ios-rounded" />
        </div>
        <div @click="goNextSlide" class="bg-[#F2E5DA] rounded-xl pt-2 px-1">
          <UIcon size="28" name="material-symbols:arrow-back-ios-new-rounded" />
        </div>
      </div>
    </div>
    <div class="mx-4 sm:mx-8 md:mx-14 mt-6 md:mt-10">
      <Swiper
        ref="swiperRef"
        :modules="[SwiperAutoplay]"
        :slides-per-view="2"
        :breakpoints="categoryBreakpoints"
        :loop="false"
        :autoplay="{
          delay: 4000,
          disableOnInteraction: true,
        }"
        @swiper="onSwiper"
      >
        <SwiperSlide class="text-center" v-for="item in category" :key="item.title">
          <div class="flex flex-col items-center">
            <div
              class="group border-2 w-1/3 py-4 rounded-lg hover:bg-black duration-300 max-xl:w-1/2"
              @click="categoryLink(item.link)"
            >
              <UIcon
                class="mt-2 group-hover:bg-white duration-300"
                size="38"
                :name="item.Icon"
              />
            </div>
            <h3 class="mt-3">{{ item.title }}</h3>
          </div>
        </SwiperSlide>
      </Swiper>
    </div>
  </div>
</template>
<script setup>
const swiperRef = ref(null)
const categoryBreakpoints = {
  640: {
    slidesPerView: 3
  },
  1024: {
    slidesPerView: 6
  }
}
const category = [
  { Icon: "ph:coffee-bean-bold", title: "قهوه ساز ها", link: "/" },
  { Icon: "material-symbols:blender", title: "آسیاب قهوه ", link: "/" },
  { Icon: "mdi:shaker", title: "ابزار باریستا", link: "/" },
  { Icon: "line-md:coffee-loop", title: "دم آوری قهوه", link: "/" },
  { Icon: "pepicons-pencil:soft-drink", title: "تجهیزات بار سرد", link: "/" },
  { Icon: "material-symbols:microwave-gen", title: "کرپ ساز صنعتی", link: "/" },
  { Icon: "mdi:kettle-steam-outline", title: "بویلر آب جوش ", link: "/" },
  { Icon: "ri:cake-3-line", title: "شو کیک", link: "/" },
];

const categoryLink = (link) => {
  navigateTo(link);
};

const onSwiper = (swiperInstance) => {
  swiperRef.value = swiperInstance;
};

const goPrevSlide = () => {
  if (swiperRef.value) {
    swiperRef.value.slidePrev();
  }
};

const goNextSlide = () => {
  if (swiperRef.value) {
    swiperRef.value.slideNext();
  }
};


</script>
