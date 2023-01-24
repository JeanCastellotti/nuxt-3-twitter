<script setup>
defineProps({
  title: String,
})
</script>

<template>
  <div
    class="m-2 overflow-hidden rounded-2xl border border-gray-200 bg-gray-50 dark:border-none dark:bg-slate-700"
  >
    <h1
      class="border-b border-gray-200 p-3 font-semibold text-slate-800 dark:border-none dark:text-slate-100"
    >
      {{ title }}
    </h1>
    <slot />
    <div
      class="cursor-pointer p-3 text-sm text-blue-400 transition hover:bg-gray-100 dark:hover:bg-slate-600"
    >
      Show more
    </div>
  </div>
</template>
