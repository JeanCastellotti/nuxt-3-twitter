<script setup>
const darkMode = ref(true)
</script>

<template>
  <div :class="{ dark: darkMode }">
    <div class="min-h-screen bg-white dark:bg-slate-800">
      <div
        class="mx-auto grid grid-cols-12 sm:px-6 lg:max-w-7xl lg:gap-5 lg:px-8"
      >
        <SidebarLeft />
      </div>
    </div>
  </div>
</template>
