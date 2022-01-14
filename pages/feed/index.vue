<template>
  <main>
    <h1>Feed</h1>
    <ul>
      <li 
        class="post"
        v-for="post in posts"
        :key="post.slug"
      >
        <nuxt-link
          :to="post.path"
          v-html="post.title"
        />
      </li>
    </ul>
  </main>
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

<style scoped lang="scss">

  .post {
    list-style: none;
    padding: 16px;
    margin: 16px 0;
    border-radius: 8px;
    border: 2px solid black;
  }
</style>