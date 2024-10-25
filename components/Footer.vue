<template>
  <div>
    <div class="bg-[#28221E] flex justify-center text-white py-10">
      <div class="px-10 flex flex-col items-center">
        <div class="flex text-2xl font-extrabold">
          اریک کافه
          <NuxtImg
            class="-translate-y-3 translate-x-2 w-8 h-7"
            src="/leaf.png"
          />
        </div>
        <h3 class="text-center font-normal mt-2">
          لورم ایپسوم متن ساختگی برای طراحان میباشد که با استفاده از<br />
          آن متن تستی مینویسند!
        </h3>
        <ul class="flex gap-10 list-disc text-sm mt-5">
          <li>دسته بندی کلی یک</li>
          <li>دسته بندی کلی یک</li>
          <li>دسته بندی کلی یک</li>
          <li>دسته بندی کلی یک</li>
          <li>دسته بندی کلی یک</li>
          <li>دسته بندی کلی یک</li>
        </ul>
        <UDivider class="mt-5 opacity-10" />

        <div class="flex gap-48 mt-5">
          <div class="flex flex-col justify-center gap-5">
          <h1 class="flex items-center "><UIcon class="ml-2" name="material-symbols:call-outline"/>12345678 <span class="text-Primary">-021</span></h1>
          <h1 class="flex items-center "><UIcon class="ml-2" name="ic:baseline-gps-fixed"/> تهران خیابان تهرانی کوچه تهران پلاک ۱۲</h1>
          </div>

          <div class="flex">
          <NuxtImg class="w-20" src="/enemad.png" />
          <NuxtImg class="w-20" src="/zpal.png" />
          </div>
        </div>
      </div>
    </div>

    <div
      class="flex items-center justify-between px-10 py-2 bg-[#1E1E1E] text-white"
    >
      <h4 class="flex items-center gap-1 font-light">
        <UIcon name="lucide:copyright" />تمام حقوق این وب سایت متعلق به قهوه
        اریک میباشد
      </h4>

      <div class="flex items-center gap-3">
        <UIcon size="25" name="proicons:facebook" />
        <UIcon size="25" name="ph:whatsapp-logo" />
        <UIcon size="25" name="hugeicons:instagram" />
      </div>
    </div>
  </div>
</template>
