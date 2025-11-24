<script setup lang="ts">
import MyButton from '@/components/MyButton.vue'
import MySimpsons from '@/components/MySimpsons.vue'
</script>

<template>
  <main>
    <h1>Welcome to the Home Page</h1>

    <MyButton href="/about">Click me 1</MyButton>
    <MyButton href="/about" variant="outline">Click me 1 Outline</MyButton>
    <MyButton href="/about" variant="outline" size="small">Click me Outline small</MyButton>
    <MyButton href="/about" size="small">Click me small</MyButton>
    <MyButton>Click me 2</MyButton>

    <MySimpsons />
  </main>
</template>
