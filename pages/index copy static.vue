<template>
  <h1>{{ title }}</h1>
</template>

<script>
export default {
  // 当页面被访问时，asyncData方法会在服务器端执行，并将返回的数据注入到组件的data中。在客户端渲染时，asyncData方法会在组件切换前执行，并且不会重新请求数据。这可以提高应用程序的性能并提高用户体验。
  asyncData() {
    return { title: 'Hello world!' }
  }
}
</script>
