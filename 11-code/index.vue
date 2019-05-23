<template>
  <div>
    <Header />
    <p>Bem vindo ao FEMUG</p>
  </div>
</template>

<script>
import Header from '@/styleguide/Header'

export default {
  name: 'About',
  components: {
    Header
  }
}
</script>

<style scoped>
  p {
    text-align: center;
    font-size: 50px;
  }
</style>