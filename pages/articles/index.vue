<template>
    <div>
        <p>test</p>
    </div>
</template>

<script setup>
    const { data:articles } = await useFetch('http://localhost:8000/api/v1/articles')
</script>