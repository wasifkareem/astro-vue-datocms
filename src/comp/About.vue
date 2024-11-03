<template>
  <section class="flex bg-[#F3F1ED] w-full justify-center pt-20 px-20">
    <div class="grid grid-cols-9 items-start p-10">
      <div class="col-span-8 flex flex-col text-xl text-gray-600">
        <h2 class="text-[#4B4B4B] text-3xl font-semibold my-3">
          {{ data.aboutHeading }}
        </h2>
        <p class="my-8">{{ data.aboutPara }}</p>

        <ul v-html="data.aboutPoints" class="custom-list"></ul>
      </div>
    </div>
    <div class="col-span-3">
      <img
        class="h-80 w-[1600px] object-cover object-left mt-10 shadow-lg shadow-orange-200 rounded-lg"
        :src="data.aboutImg.url"
        alt=""
      />
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";
import VueMarkdown from "@adapttive/vue-markdown";
const markdownContent = ref("");
const props = defineProps({
  data: {
    type: Object,
    required: true,
  },
});
</script>

<style>
.custom-list li {
  margin-bottom: 1.2rem; /* Adjust spacing as needed */
}
</style>
