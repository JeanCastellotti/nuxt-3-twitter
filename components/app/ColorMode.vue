<script setup>
const darkMode = ref(false)

function toggleDarkMode() {
  darkMode.value = !darkMode.value
}

provide('toggleDarkMode', toggleDarkMode)
</script>

<template>
  <div :class="{ dark: darkMode }">
    <slot />
  </div>
</template>
