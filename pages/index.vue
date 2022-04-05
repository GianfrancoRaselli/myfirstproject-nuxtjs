<template>
  <h1>Welcome to my first nuxt app</h1>
</template>

<script>
export default {
  name: 'IndexPage',
  
  head() {
    return {
      title: 'Application Nuxt Posts | Home',
      meta: [
        {
          hid: 'index',
          name: 'index',
          content: 'Website about posts'
        }
      ],
      htmlAttrs: {
        lang: 'en'
      }
    }
  }
}
</script>
