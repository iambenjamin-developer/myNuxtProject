<template>
    <article class="blog-item">
        <h2>{{ post.title }}</h2>
        <p>{{ post.description }}</p>
        <small>ID: {{ post.id }}</small>
    </article>
</template>

<script setup lang="ts">
// Define las props con TypeScript
interface Post {
    id: number
    title: string
    description: string
}

const props = defineProps<{
    post: Post
}>()
</script>

<style scoped>
.blog-item {
    border: 1px solid #ddd;
    padding: 1rem;
    margin-bottom: 1rem;
    border-radius: 8px;
}
</style>