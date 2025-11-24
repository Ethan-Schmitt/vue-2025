<script setup lang="ts">
import MyButton from '@/components/MyButton.vue'
import MySimpsons from '@/components/MySimpsons.vue'
import MyTitle from '@/components/MyTitle.vue'
import MyForm from '@/components/MyForm.vue'
</script>

<template>
  <main>
    <MyTitle as="h1">Homepage</MyTitle>

    <MyForm />

    <!-- <MyButton href="/about">Click me 1</MyButton>
    <MyButton href="/about" variant="outline">Click me 1 Outline</MyButton>
    <MyButton href="/about" variant="outline" size="small">Click me Outline small</MyButton>
    <MyButton href="/about" size="small">Click me small</MyButton>
    <MyButton>Click me 2</MyButton>

    <MySimpsons /> -->
  </main>
</template>
