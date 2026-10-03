<script setup lang="ts">
   const {data: user} = useFetch('https://api.github.com/users/mojombo');
</script>
<template>
    <h1>Github User: {{ user?.name||'N/A' }}</h1>
</template>