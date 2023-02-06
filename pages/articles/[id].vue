<script setup>
//first create virtual host with laragon
  const {data: articles} = await useFetch('http://blog-api.test/api/v1/articles')
</script>

<template>
  <div>
    <p>test</p>
    <div>{{ articles }}</div>
  </div>
</template>