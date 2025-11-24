<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import MyHeader from './components/MyHeader.vue'
</script>

<template>
  <header>
    <MyHeader />
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
    </nav>
  </header>
  <RouterView />
</template>
