<template>
  <div>
    <h1>Nuxt stars: {{ stars }}</h1>
  </div>
</template>

<script>
export default {
  name: 'Home',
  async asyncData() {
    const res = await fetch('https://api.github.com/repos/nuxt/nuxt.js')
    const json = await res.json()
    return { stars: json.stargazers_count }
  }
}
</script>


<style scoped>
  div {
    display: grid;
    justify-content: center;
    color: red;
  }
</style>