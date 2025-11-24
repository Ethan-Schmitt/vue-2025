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
.button {
  padding: 10px 20px;
  background: black;
  color: white;
  border: none;
  border-radius: 4px;
}
</style>
