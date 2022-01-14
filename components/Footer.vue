<template>
  <footer>
    <p>&copy; {{currentYear}}</p>
    <nav>
      <a href="https://github.com/izzee/nuxtlify" target="_blank">Repo</a>
    </nav>
  </footer>
</template>

<script>
export default {
  computed: {
    currentYear(){ return new Date().getFullYear()}
  }
}
</script>

<style scoped lang="scss">
  footer {
    padding: 16px;
    border: 2px solid $black;
    border-radius: 8px;
    display: flex;
    align-items: center;
  }
  nav {
    flex: 1;
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }
</style>