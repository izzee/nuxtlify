<template>
  <div>
    <NuxtLink
      v-for="post in posts"
      :key="post.slug"
      :to="post.path"
      v-html="post.title"
    />
  </div>
</template>

<script>
export default {
  async asyncData ({ $content }) {
    const posts = await $content('feed').fetch()
    return {
      posts
    }
  }
}
</script>

<style>


</style>