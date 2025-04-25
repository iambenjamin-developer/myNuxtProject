<template>
    <div>
        <h1>About page</h1>
        <h2>{{ user.name.first }} {{ user.name.last }}</h2>
    </div>
</template>

<script setup lang="ts">
import type { User } from '~~/interfaces/user';

const { data, pending, error, refresh } = await useFetch('https://randomuser.me/api/')

const user = computed(() => {
    const d = data.value as User
    return d.results[0]
});

</script>


<style scoped></style>