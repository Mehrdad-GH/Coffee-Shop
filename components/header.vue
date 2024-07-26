<template>
  <div class="mx-20">
    <div class="flex justify-between  my-5">
      <div class="flex">
        <h1 class="ml-1 text-end">
          <span class="color-primary">-۰۲۱</span><br />
          ۱۲۳۴۵۲۱۶۲
        </h1>
        <img src="/icons/coffee.png" alt="" />
      </div>

      <div>
        <img src="/icons/Logo.png" alt="" />
      </div>

      <div class=" ">
        <button
          class="border-2 border-black p-3 rounded-full hover:bg-black hover:text-white duration-200"
        >
          ورود / ثبت نام
        </button>

        <button
          class="border-2 bg-[#9E624C] text-white border-black mr-5 p-4 rounded-full hover:bg-white hover:text-[#9E624C] duration-200"
        >
          <font-awesome class="text-2xl" transform="down-2 right-1" :icon="faCartShopping" />
        </button>
      </div>
    </div>


    <div class="flex justify-between items-center bg-[#28221E] rounded-full w-full text-white">
      <ul class="flex gap-10 p-5">
        <li>صفحه اصلی</li>
        <li>محصولات</li>
        <li>خدمات</li>
        <li>آموزش ها</li>
        <li> درباره ما</li>
        <li> تماس با ما</li>
      </ul>

      <div class="bg-white/20 flex rounded-full gap-2 p-2 ml-5 ">
          <h3 class="mt-1">Eric.Cafe</h3>
          <font-awesome class="text-3xl  ml-1"  :icon="faInstagram" />
      </div>


    </div>
  </div>
</template>

<script setup>
import { faCartShopping  } from '@fortawesome/free-solid-svg-icons'
import {faInstagram} from '@fortawesome/free-brands-svg-icons'


</script>

<style></style>
