<template>
  <div class="w-screen p-2 py-3 flex justify-center">
    <nav>
      <ul class="flex gap-3">
        <li
          class="border border-slate-400 hover:border-slate-500 text-slate-400 hover:text-slate-500 px-2 py-1 rounded-lg transition-all duration-200"
        >
          <a href="/">Home</a>
        </li>
        <li
          class="border border-slate-400 hover:border-slate-500 text-slate-400 hover:text-slate-500 px-2 py-1 rounded-lg transition-all duration-200"
        >
          <a href="/about">About</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
</script>
