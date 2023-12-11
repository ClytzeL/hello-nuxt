<template>
  <ul>
    <li v-for="post in posts" :key="post.id">{{ post.title }}</li>
  </ul>
</template>

<script>
export default {
  async asyncData({ $axios }) {
    const response = await $axios.get('https://jsonplaceholder.typicode.com/posts')
    return { posts: response.data }
  }
}
</script>
