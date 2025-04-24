<template>
    <div>
        <h1>Blog Post</h1>

        <ul>
            <li v-for="item in list" :key="item.id">
                {{ item.title }}
            </li>
        </ul>
    </div>
</template>

<script setup lang="ts">

const list = ref([
    {
        id: 1,
        title: 'Brasil',
        description: 'Carnaval, parintis'
    },
    {
        id: 2,
        title: 'Argentina',
        description: 'Chalten'
    },
    {
        id: 3,
        title: 'Japon',
        description: 'Tokio'
    },
]);
</script>

<style scoped></style>