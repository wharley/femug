<template>
  <div class='container'>
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'Container'
}
</script>

<style scoped>
  .container {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    grid-gap: 20px;
  }
</style>