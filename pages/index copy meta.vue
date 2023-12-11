<template>
  <div>
    <h1>{{ title }}</h1>
    <p>{{ description }}</p>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: this.title,
      meta: [
        { hid: 'description', name: 'description', content: this.description }
      ]
    }
  },

  data() {
    return {
      title: 'My Page',
      description: 'Here is a short description of my page.'
    }
  }
}
</script>
