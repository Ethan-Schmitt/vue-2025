<script setup lang="ts">
defineProps<{
  prenom: string
  nom: string
  description: string
  img: string
}>()
</script>
<template>
  <div class="character">
    <img :src="`/images/${img}`" />
    <h3>{{ prenom }} {{ nom }}</h3>
    <p>{{ description }}</p>
  </div>
</template>
<style lang="scss">
.character {
  max-width: rem(300);
  padding: rem(16);
}
</style>
