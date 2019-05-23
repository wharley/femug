<template>
  <div>
    <h4>{{ user }}</h4>
    <a href='url' target='_blank'>{{ url }}</a>
  </div>
</template>

<script>
export default {
  name: 'CardTitle',
  props: [ 'user', 'url' ]
}
</script>

<style scoped>
  a {
    text-decoration: none;
  }
</style>