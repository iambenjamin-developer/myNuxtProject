import { NuxtLink } from '../.nuxt/components';
<template>
  <div>
    <div>
      <NuxtLink to="/">Home</NuxtLink>
      <br>
      <NuxtLink to="/blog">Blog</NuxtLink>
      <br>
      <NuxtLink to="/about">About</NuxtLink>
      <br>
    </div>
    <NuxtPage />
  </div>
</template>
