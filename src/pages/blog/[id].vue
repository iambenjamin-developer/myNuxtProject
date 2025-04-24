<template>
    <div>
        <h2>{{ id }}</h2>
    </div>
</template>

<script setup lang="ts">
// ✅ Correcto: useRoute() dentro de <script setup>
const route = useRoute()
const id = route.params.id  // Accede al parámetro dinámico
</script>