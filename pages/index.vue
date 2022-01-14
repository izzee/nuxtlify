<template>
<main>
  <h1>Home</h1>
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
