<script setup>
import { Layout, Typography, Image } from 'ant-design-vue';
const { Title } = Typography;
const { Content } = Layout;

const volunteerList = [
  'Jackson Davis',
  'Elias Gillete',
  'Freya Moore',
  'Elvira Montanez',
  'Herman Adelphi',
];
</script>

<template>
  <Layout class="layout">
    <Content class="content">
      <div class="first-half">
        <Title :level="2">Meet Our Intrepid Rescue Leaders</Title>
      </div>
      <div class="second-half">
        <div v-for="volunteer in volunteerList" :key="volunteer">
          <Image :style="{ borderRadius: '50%', objectFit: 'cover'}" width="6rem" height="6rem" :preview="false" :src="'/assets/' + volunteer.replace(' ','-') + '.jpg'">
          </Image>
          {{ volunteer }}
        </div>
      </div>
    </Content>
  </Layout>
</template>

<style lang="scss" scoped>
.layout,
.content {
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
  background-color: #ddf1cf;
}
.first-half h2 {
  font-size: 4.5rem;
  width: 85%;
  padding: 0 5rem;
}
.first-half,
.second-half {
  width: 50%;
  height: 100vh;
}
.second-half {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  padding: 4rem 0;
}
</style>
