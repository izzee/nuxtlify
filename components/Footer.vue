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
    box-shadow: 0 0 0 2px $black;
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
  a, p { 
    line-height: 1; 
    font-size: 16px;
  }
</style>