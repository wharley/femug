<template>
  <div>
    <Header />
    <Title title='Lista de usuários - GITHUB' />
    <Container>
      <Card :key='user.id' v-for='user in users'>
        <layout-image :src='user.avatar_url' alt='avatar' />
        <Content>
          <card-title :user='user.login' :url='user.html_url' />
        </Content>
      </Card>
    </Container>
  </div>
</template>

<script>
import Container from '@/styleguide/Container'
import Card from '@/styleguide/Card'
import CardTitle from '@/styleguide/CardTitle'
import Content from '@/styleguide/Content'
import LayoutImage from '@/styleguide/Image'
import Title from '@/styleguide/Title'

import Header from '@/styleguide/Header'

export default {
  name: 'Home',
  components: {
    Container,
    Card,
    CardTitle,
    Content,
    LayoutImage,
    Title,
    Header
  },
  async asyncData() {
    const res = await fetch('https://api.github.com/users')
    const json = await res.json()
    return { users: json }
  }
}
</script>