<script setup lang="ts">
defineProps<{
  href?: string
  variant?: 'default' | 'outline'
}>()
</script>

<template>
  <a v-if="href" href="" class="button" :class="{ '-outline': variant === 'outline' }"
    ><slot></slot
  ></a>
  <button v-else class="button" :class="{ '-outline': variant === 'outline' }">
    <slot></slot>
  </button>
</template>

<style lang="scss">
@use '@/assets/foundations/functions' as *;
.button {
  --button-color: var(--color-text);
  --button-bg-color: var(--color-primary);
  --button-border-color: var(--color-primary);
  padding: rem(10) rem(20);
  background: var(--button-bg-color);
  color: var(--button-color);
  border: rem(1) solid var(--button-border-color);
  border-radius: rem(4);
  text-decoration: none;
  font-size: var(--font-size-base);
  &:hover {
    --button-color: var(--color-primary);
    --button-bg-color: transparent;
  }
  &.-outline {
    --button-color: var(--color-primary);
    --button-bg-color: transparent;
    &:hover {
      --button-color: var(--color-text);
      --button-bg-color: var(--color-primary);
    }
  }
}
</style>
