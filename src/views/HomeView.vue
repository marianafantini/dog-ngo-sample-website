<script setup>
import { Layout, Typography, Button } from 'ant-design-vue';
const { Title } = Typography;
const { Content } = Layout;
</script>

<template>
  <Layout class="layout">
    <Content>
      <Title :level="1">Our four-legged friends need your help</Title>
      <Title :level="4">Quest for Paws Animal Rescue and Sanctuary</Title>
      <Button size="large">Sponsor a rescue today</Button>
    </Content>
  </Layout>
</template>

<style scoped>
.layout {
  background-image: url('../../public/assets/home.jpeg');
  background-size: 100% auto;
  background-repeat: no-repeat;
  width: 100%;
  height: 100vh;
  display: flex;
  flex-direction: row;
  align-items: center;
}
h1,
h4 {
  color: whitesmoke;
  margin: 0 5rem;
  max-width: 27%;
}
h1 {
  font-size: 4rem;
}
button {
  margin: 2rem 5rem;
  background-color: #ddf1cf;
  border-color: #ddf1cf;
  font-weight: bold;
  font-size: 1rem !important;

  &:hover {
    color: #0a3162;
    border-color: #0a3162;
  }
}
</style>
