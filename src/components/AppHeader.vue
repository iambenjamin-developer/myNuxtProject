<template>
    <div>
        <NuxtLink to="/">Home</NuxtLink>
        <br>
        <NuxtLink to="/blog">Blog</NuxtLink>
        <br>
        <NuxtLink to="/about">About</NuxtLink>
        <br>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    setup() {


        return {}
    }
})
</script>

<style scoped></style>