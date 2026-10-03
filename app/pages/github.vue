<script setup lang="ts">
   const {data: users} = useFetch('https://api.github.com/users') ;
</script>
<template>
    <h1>Github Users</h1>

    <div v-for="user in users" >
        <h1>{{ user.login }}</h1>
      <p>ID is: {{ user?.id||'N/A' }}</p>
      <p>{{ user?.name||'N/A' }}</p>
    </div>
</template>