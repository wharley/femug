<template>
  <div class='card'>
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'Card'
}
</script>

<style scoped>
  .card {
    border: 1px solid #d3d3d3;
    border-radius: 0.25rem;
  }
</style>