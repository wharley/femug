<template>
  <div class='title'>
    <h1>{{ title }}</h1>
  </div>
</template>

<script>
export default {
  name: 'Title',
  props: [ 'title' ]
}
</script>

<style scoped>
  h1 {
    display: grid;
    justify-content: center;
    color: #fff;
  }
  .title {
    display: grid;
    padding: 0 15px;
    margin-bottom: 1rem;

    background-color: #24292e;
  }
</style>