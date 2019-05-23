<template>
  <nav>
    <nuxt-link to='/'>Home</nuxt-link>
    <nuxt-link to='/about'>About</nuxt-link>
  </nav>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped>
  nav {
    text-align: center;
    margin-top: 1rem;
    margin-bottom: 1rem;
  }
  a {
    margin-right: 1rem;
  }
</style>