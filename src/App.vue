<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import MyHeader from './components/MyHeader.vue'
import DefaultLayout from './layouts/DefaultLayout.vue'
</script>

<template>
  <DefaultLayout>
    <template #header>
      <MyHeader />
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </template>
    <RouterView />
    <template #aside>
      <p>Aside</p>
    </template>
    <template #footer>
      <p>Footer</p>
    </template>
    <p>paragraphe</p>
  </DefaultLayout>
</template>
