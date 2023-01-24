<script setup>
const props = defineProps({
  active: {
    type: Boolean,
    default: false,
  },
})

const textWeight = computed(() => ({
  'font-semibold': props.active,
  'font-normal': !props.active,
}))

const textColor = computed(() => ({
  'text-slate-700': props.active,
  'text-slate-500': !props.active,
  'dark:text-slate-100': props.active,
  'dark:text-slate-400': !props.active,
}))
</script>

<template>
  <NuxtLink
    to="/"
    class="flex w-min items-center gap-4 rounded-full p-3 transition hover:bg-gray-100 dark:hover:bg-slate-700"
    :class="textColor"
  >
    <slot name="icon" />
    <span class="hidden text-xl xl:block" :class="textWeight">
      <slot name="label" />
    </span>
  </NuxtLink>
</template>
