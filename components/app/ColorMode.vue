<script setup>
const darkMode = ref(false)
</script>

<template>
  <div :class="{ dark: darkMode }">
    <slot />
  </div>
</template>
