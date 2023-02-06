<script setup>
//first create virtual host with laragon
  const {data: articles} = await useFetch('http://blog-api.test/api/v1/articles')

  let isLoading = ref(false)

  function onSubmit() {

  }

</script>

<template>
  <div>
    <h2>Article creation</h2>
    <div>
      <form @submit.prevent="onSubmit">
        <fieldset>
          <div>
            <label for="title">Title</label>
            <input type="text" id="title" name="title">
          </div>

          <div>
            <label for="content">Content</label>
            <textarea id="content" name="content"></textarea>
          </div>

          <button type="submit">Create</button>
        </fieldset>
      </form>
    </div>
  </div>
</template>