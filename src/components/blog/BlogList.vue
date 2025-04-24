<template>
  <div class="blog-list">
    <h1>Lista de Blogs</h1>
    <BlogItem v-for="post in posts" :key="post.id" :post="post" />
  </div>
</template>

<script setup lang="ts">
import type { Post } from './BlogItem.vue'

// Datos estáticos (puedes reemplazar por datos de API)
const posts: Post[] = [
  {
    id: 1,
    title: 'Introducción a Nuxt 3',
    description: 'Aprende los fundamentos de Nuxt 3'
  },
  {
    id: 2,
    title: 'Vue Composition API',
    description: 'Domina la Composition API en Vue'
  }
]
</script>