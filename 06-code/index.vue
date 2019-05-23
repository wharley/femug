<template>
  <img src='src' alt='alt' />
</template>

<script>
export default {
  name: 'LayoutImage',
  props: [ 'src', 'alt' ]
}
</script>

<style scoped>
  img {
    width: 300px;
    height: 100px;
    background-size: cover;

    min-height: 180px;
    background-position: center;
    background-color: #ccc;
  }
</style>