<template>
<main>
  <h1>Home</h1>
  <p>A Nuxt simple template for blogs, galleries, and portfolios built using:</p>
  <ul>
    <li>Nuxt Content</li>
    <li>Nuxt Image</li>
    <li>Netlify CMS</li>
    <li>Netlify Large Media</li>
  </ul>

</main>
</template>

<script>
  export default {
    head() {
      return {
        script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
      };
    },
  };
</script>

<style lang="scss" scoped>
main > * + * {
  margin-top: 16px;
}
ul li {
  list-style-position: inside;
  margin-top: 8px;
}
</style>