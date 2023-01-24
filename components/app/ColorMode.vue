<script setup>
const darkMode = ref(true)
</script>

<template>
  <div :class="{ dark: darkMode }">
    <slot />
  </div>
</template>
