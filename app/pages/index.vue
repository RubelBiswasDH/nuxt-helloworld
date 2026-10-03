<script setup lang="ts">
    useHead({
        title: "Home Page",
        meta: [
            {
                name: "description",
                content: "This is the home page of our Nuxt3 application."
            }
        ]
    })

    const {data} = useFetch("/api/userdetails")
</script>
<template>
    <h1>Home Page</h1>
    <p>{{ data?.msg }}</p> 
    <NuxtLink to="/about">Go to About Page</NuxtLink>
</template>