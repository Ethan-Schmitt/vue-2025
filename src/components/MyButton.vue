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
  padding: rem(10) rem(20);
  background: black;
  color: white;
  border: none;
  border-radius: 4px;
}
</style>
