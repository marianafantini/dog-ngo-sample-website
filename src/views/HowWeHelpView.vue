<script setup>
import { Layout, Typography, Image } from 'ant-design-vue';
const { Title, Paragraph } = Typography;
const { Content } = Layout;
</script>

<template>
  <Layout class="layout">
    <Content class="content">
      <Title :level="2">How We Help</Title>

      <div class="flex">
        <div>
          <Image height="7rem" :preview="false" src="/assets/dog-icon.png"></Image>
          <Title :level="4">Animal Rescue</Title>
          <Paragraph>
            We go on quests to rescue and recover any dog or cat roaming our streets.
          </Paragraph>
        </div>
        <div>
          <Image height="7rem" :preview="false" src="/assets/vet-icon.png"></Image>
          <Title :level="4">Veterinary Services</Title>
          <Paragraph>
            We provide free veterinary treatment to strays, rescues, and pets.
          </Paragraph>
        </div>
        <div>
          <Image height="7rem" :preview="false" src="/assets/home-icon.png"></Image>
          <Title :level="4">Fostering and Adoption</Title>
          <Paragraph> We help our rescues find their temporary and forever homes. </Paragraph>
        </div>
      </div>
    </Content>
  </Layout>
</template>

<style lang="scss" scoped>
.layout {
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
  background-color: #a5b5eb;
}
h2 {
  font-size: 4.5rem;
  padding: 3rem;
}
.content {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.flex {
  display: flex;
  justify-content: space-around;
  padding: 4rem;
  font-weight: 400;

  div {
    max-width: 80%
  }
}
</style>
