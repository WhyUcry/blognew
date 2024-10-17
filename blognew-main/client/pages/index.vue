<template>
    <h2>Главная страница</h2>

    

    


</template>

<script setup>
    
const { id } = useRoute().params 

const api = await $fetch(`http://localhost:1337/api/blogs?populate=*`)
// const post = api.data[id]
// const mark = post.body

const base_url = 'http://localhost:1337'
</script>

<style scoped>
    template {
    }
</style>