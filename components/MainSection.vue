<script setup>
defineProps({
  title: String,
  loading: Boolean,
})
</script>

<template>
  <div>
    <div
      class="sticky top-0 bg-white/80 px-4 py-3 backdrop-blur-md dark:bg-slate-800/80"
    >
      <h2 class="text-xl font-semibold text-slate-800 dark:text-slate-100">
        {{ title }}
      </h2>
    </div>
    <div v-if="loading">Loading...</div>
    <slot v-else />
  </div>
</template>
