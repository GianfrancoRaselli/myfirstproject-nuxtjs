<template>
  <div>
    <h1>About Us</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, temporibus vel ducimus nam iste adipisci error fuga similique accusantium repellendus delectus eius sit dignissimos iusto maiores assumenda porro sapiente architecto.</p>
  </div>
</template>

<script>
export default {
  name: 'AboutPage',
  
  head() {
    return {
      title: 'Application Nuxt Posts | About',
      meta: [
        {
          hid: 'about',
          name: 'about',
          content: 'About Us Page'
        }
      ],
      htmlAttrs: {
        lang: 'en'
      }
    }
  }
}
</script>