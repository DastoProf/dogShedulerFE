<script setup>
const { data: users } = useFetch("https://jsonplaceholder.typicode.com/users");
</script>

<template>
  <section>
    <p>This page will be displayed at the /about route.</p>
    <ul>
      <li v-for="user in users">{{ user.name }}</li>
    </ul>
  </section>
</template>
