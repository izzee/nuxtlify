<template>
  <div>
    <h1>Feed</h1>
    <ul>
      <li 
        v-for="post in posts"
        :key="post.slug"
      >
        <nuxt-link
          :to="post.path"
          v-html="post.title"
        />
      </li>
    </ul>
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