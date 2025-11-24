<script setup lang="ts">
defineProps<{
  href?: string
}>()
</script>

<template>
  <a v-if="href" href="" class="button"><slot></slot></a>
  <button v-else class="button"><slot></slot></button>
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
}
</style>
