<template>
  <footer>
    <span>&copy; {{currentYear}}</span>
  </footer>
</template>

<script>
export default {
  computed: {
    currentYear(){ return new Date().getFullYear()}
  }
}
</script>
