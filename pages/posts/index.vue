<template>
  <div>
    <h1>Posts</h1>
    <Post
      v-for="post of posts"
      v-bind:key="post.id"
      :id="post.id"
      :title="post.title"
    />
  </div>
</template>

<script>
import axios from 'axios'

export default {
  head() {
    return {
      title: 'Application Nuxt Posts | Posts',
      meta: [
        {
          hid: 'posts',
          name: 'posts',
          content: 'posts'
        }
      ],
      htmlAttrs: {
        lang: 'en'
      }
    }
  },

  data() {
    return {
      posts: []
    }
  },

  async created() {
    try {
      const res = await axios.get('https://jsonplaceholder.typicode.com/posts');
      this.posts = res.data;
    } catch (err) {
      console.log(err);
    }
  }
}
</script>