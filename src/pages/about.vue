<template>
    <div>
        <h1>About page</h1>
        <h2>{{ user.name.first }} {{ user.name.last }}</h2>
        <h3>{{ user.login.password }}</h3>
        <i>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nobis facilis, amet nesciunt autem sed numquam
            eveniet nostrum dolore tempore error doloribus saepe quidem ducimus corrupti. Ducimus incidunt nostrum
            tenetur corrupti.</i>
    </div>
</template>

<script setup lang="ts">
import type { Result, User } from '~~/interfaces/user';

const { data, error, refresh } = await useFetch(`https://randomuser.me/api/`, {
    method: 'get',
    query: {
        gender: 'female',
        password: 'upper,lower,1-16'
    }
})
const user = computed<Result>(() => {
    const d = data.value as User
    return d.results[0]
});

</script>


<style scoped></style>