<template>
  <section class="h-[80vh]">
    <div class="flex flex-col items-center justify-center">
      <img
        class="w-44 border border-orange-500 border-opacity-50 rounded-full p-2 px-6 my-10"
        :src="data.logo.url"
        alt=""
      />
      <h1
        class="text-center w-[600px] text-[65px] text-black font-extrabold leading-[1.2] opacity-80 bg-gradient-to-br from-slate-900 via-orange-500 to-indigo-400 inline-block text-transparent bg-clip-text py-10"
      >
        {{ data.heading }}
      </h1>
      <p class="text-gray-500 w-[550px] text-center text-3xl">
        {{ data.subHeading }}
      </p>
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
