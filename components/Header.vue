<template>
  <div class="mt-5 mx-16 max-lg:hidden">
    <div class="flex justify-between items-center">
      <div class="text-left text-lg flex items-center">
        <h1>
          <span class="text-Primary"> -021</span><br />
          123456789
        </h1>

        <div class="bg-red-100 flex rounded-full shadow-2xl p-3 mr-4">
          <UIcon class="text-Primary" name="ph:coffee-bean-fill" size="30" />
        </div>
      </div>

      <NuxtLink to="/"><NuxtImg class="h-10" src="/logo.png" /></NuxtLink>

      <div class="flex">
        <div
          class="rounded-full px-6 py-2 my-2 border-2 border-black hover:bg-black hover:text-white duration-300"
        >
          ورود / ثبت نام
        </div>
        <UButton
          class="rounded-full bg-Primary px-3 m-2 border-2 hover:bg-white hover:text-black hover:border-black duration-500"
          icon="ic:outline-shopping-bag"
          :padded="false"
        ></UButton>
      </div>
    </div>

    <div
      class="flex justify-between items-center bg-[#28221E] text-white w-full rounded-full pr-10 mt-5 py-3 relative"
    >
      <ul class="flex gap-10">
        <li>صفحه اصلی</li>
        <li class="relative group flex">
          لیست محصولات
          <UIcon
            class="mt-1"
            name="material-symbols:keyboard-arrow-down-rounded"
          />
          <ul
            class="absolute hidden group-hover:block bg-[#38322E] mt-5 text-white rounded-lg p-3 z-10 min-w-max"
          >
            <li class="py-1 px-5 hover:bg-[#28221E] rounded">محصول ۱</li>
            <li class="py-1 px-5 hover:bg-[#28221E] rounded">محصول ۲</li>
            <li class="py-1 px-5 hover:bg-[#28221E] rounded">محصول ۳</li>
          </ul>
        </li>
        <li>خدمات</li>
        <li>آموزش ها</li>
        <li>درباره ما</li>
        <li>تماس با ما</li>
      </ul>

      <div class="flex bg-[#FFFFFF33] p-2 rounded-full ml-5 gap-2 px-3">
        <h1>Eric.Cafe</h1>
        <UIcon class="-mt-0.5" size="25" name="ph:instagram-logo-bold" />
      </div>
    </div>
  </div>

  <div class="hidden max-lg:flex justify-between mx-8 items-center">
    <button
      class="bg-[#F2E5DA] mr-7 mt-7 px-2 rounded-full border-black border-2 hover:border-[#F2E5DA] duration-500"
      @click="drawerOpen=!drawerOpen"
    >
      <UIcon class="mt-2" size="23" name="fa6-solid:bars-staggered" />
    </button>
    <NuxtLink to="/"><NuxtImg class="h-10" src="/logo.png" /></NuxtLink>
    <UButton
      class="rounded-full bg-Primary px-3 py-3 mt-5 border-2 hover:bg-white hover:text-black hover:border-black duration-500"
      icon="ic:outline-shopping-bag"
      :padded="false"
    ></UButton>
  </div>
  <div
    :class="[
      'hidden max-lg:flex fixed inset-0 z-50 duration-700',
      drawerOpen ? 'right-0' : '-right-full',
    ]"
  >
    <div class="flex w-2/3 max-w-xs h-full bg-black text-white">
      <UIcon
        size="30"
        name="material-symbols:keyboard-double-arrow-right-rounded"
        class="mt-5 ml-3 cursor-pointer"
        @click="drawerOpen = !drawerOpen"
      />
      <ul class="flex flex-col gap-7 mt-16 ml-5">
        <li class="hover:text-stone-600 duration-300">صفحه اصلی</li>
        <li class="hover:text-stone-600 duration-300">لیست محصولات</li>
        <li class="hover:text-stone-600 duration-300">خدمات</li>
        <li class="hover:text-stone-600 duration-300">آموزش ها</li>
        <li class="hover:text-stone-600 duration-300">درباره ما</li>
        <li class="hover:text-stone-600 duration-300">تماس با ما</li>
      </ul>
    </div>
  </div>
</template>

<script setup>
const drawerOpen = ref(false);
</script>
