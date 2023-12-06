<script lang="ts" setup>
import { useAttrs } from 'vue'
import { useFormField } from './useFormField'
import { cn } from '@/utils'

defineOptions({
  inheritAttrs: false,
})

const { formDescriptionId } = useFormField()
const { class: className, ...rest } = useAttrs()
</script>

<template>
  <p
    :id="formDescriptionId"
    :class="cn('text-sm text-neutral-500 dark:text-neutral-400', className ?? '')"
    v-bind="rest"
  >
    <slot />
  </p>
</template>
