<script setup lang="ts">
    definePageMeta({
        layout: 'admin'
    })

    useHead({
      title: "About Page"
    })
</script>
<template>
  <h1>About Page</h1>
  <NuxtLink to="/">Go to Home Page</NuxtLink>
</template>