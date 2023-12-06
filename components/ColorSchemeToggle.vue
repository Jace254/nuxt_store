<script lang="ts" setup>
const color = useColorMode()

function toggleDark() {
  color.value = color.value === 'dark'
    ? 'light'
    : 'dark'
}
</script>

<template>
  <button
    rounded p-2
    hover="bg-active"
    @click="toggleDark"
  >
    <div dark:i-ph-sun-dim-duotone i-ph-moon-stars-duotone text-2xl />
  </button>
</template>
