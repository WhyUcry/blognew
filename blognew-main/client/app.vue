<template>
  <Navbar />
  <NuxtPage />
  <Footer />
</template>

<script setup>
const { id } = useRoute().params 

const api = await $fetch(`http://localhost:1337/api/blogs?populate=*`)
// const posts = api.data
// const mark = posts.body

const base_url = 'http://localhost:1337'
</script>

<style>
  html, body, #__nuxt {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
  }

  main {
    flex: 1 1 auto;
  }
</style>