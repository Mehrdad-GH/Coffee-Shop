<template>
  <div class="mx-4 sm:mx-10 lg:mx-20 flex flex-col lg:flex-row gap-5 mt-5 text-white">
    <div
      class="bg-[#28221E] flex flex-col justify-between w-full lg:w-1/4 rounded-lg py-10 lg:py-20 px-8 lg:px-12 max-xl:w-1/3 max-lg:px-6 max-lg:gap-4"
    >
      <div class="flex text-4xl font-extrabold max-xl:text-3xl">
        اریک کافه
      </div>

      <div class="text-right text-md font-light">
        کامل ترین تجهیزات کافه و رستوران در ایران
      </div>

      <UButton
        class="rounded-full px-5 mx-5 flex justify-between bg-white/20 hover:bg-white/25 duration-200 max-xl:mx-2 max-xl:px-3 max-xl:mt-2 max-lg:px-2"
      >
        مشاهده محصولات
        <UIcon size="25" name="material-symbols-light:arrow-left-alt-rounded" />
      </UButton>
    </div>

    <div class="bg-[#847669] w-full lg:w-3/4 rounded-lg flex justify-start items-end max-xl:w-2/3 mt-4 lg:mt-0">
      <div
        class="flex flex-col self-center gap-5 mr-6 lg:mr-20 font-bold text-3xl lg:text-4xl whitespace-nowrap "
      >
        <h2>کافه از تو</h2>
        <h4>تجهیزات با ما</h4>
        <nuxt-link to="/"
          ><UIcon
            class="hover:w-14 hover:text-white/30 duration-300"
            name="material-symbols-light:arrow-left-alt-rounded"
        /></nuxt-link>
      </div>

      <div class="flex justify-end w-full">
        <NuxtImg class="w-4/6 max-lg:w-full" src="/hand.png" />
      </div>
    </div>
  </div>



<div class="absolute left-0 -mt-56  opacity-10 z-10">
<NuxtImg class="w-20" src="/treeShape.png" />
</div>

<NuxtImg class="relative mt-16 z-20" src="/serperator.png" />


</template>
