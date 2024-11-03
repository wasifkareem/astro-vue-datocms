<template>
  <section class="bg-[#FAF7F2] flex w-full justify-center pt-20">
    <div class="grid grid-cols-9 items-start w-full p-10 gap-4">
      <div class="col-span-4 flex justify-center">
        <img class="rounded-lg h-[450px]" :src="data.introImg.url" alt="" />
      </div>
      <div class="col-span-4 flex flex-col gap-5">
        <h2 class="text-6xl w-[480px] mb-4 font-semibold text-[#4B4B4B]">
          {{ data.heading }}
        </h2>
        <p class="text-xl text-gray-700">{{ data.para }}</p>
        <p class="text-lg text-gray-500">{{ data.paratwo }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
const props = defineProps({
  data: {
    type: Object,
    required: true,
  },
});
</script>

<style scoped></style>
