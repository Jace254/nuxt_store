<script lang="ts" setup>
const colorMode = useColorMode()

function toggleMode() {
  colorMode.preference = colorMode.value === 'light' ? 'dark' : 'light'
}
</script>

<template>
  <button
    rounded p-2
    hover="bg-active"
    @click="toggleMode"
  >
    <div dark:i-ph-sun-dim-duotone i-ph-moon-stars-duotone text-2xl />
  </button>
</template>
