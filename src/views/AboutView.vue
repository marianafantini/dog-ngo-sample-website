<script setup>
import { Layout, Typography, Image } from 'ant-design-vue';
const { Title, Paragraph } = Typography;

const { Content } = Layout;
</script>

<template>
  <Layout class="layout">
    <Content class="content">
      <div class="first-half">
        <Title :level="2" class="first-title">Pets change our lives.</Title>
        <Title :level="2" class="second-title">We're on a quest to change theirs.</Title>
        <Paragraph class="paragraph">
          Quest for Paws Animal Rescue and Sanctuary is a nonprofit organization dedicated to
          rescuing, fostering, and rehoming the abandoned, sick, and injured animals around our
          city.
        </Paragraph>
        <Paragraph class="paragraph">
          With you help, we hope to make a difference in the lives of these wonderful animals.
        </Paragraph>
      </div>
      <div class="second-half">
        <Image class="image" :style="{ borderRadius: '5rem'}" width="80%" :preview="false" src="./assets/about.jpeg"></Image>
      </div>
    </Content>
  </Layout>
</template>

<style lang="scss" scoped>
.image {
  border-radius: 1rem;
}
.content {
  display: flex;
  width: 100%;
}
.first-half {
  background-color: #1c7c54;
}
.second-half {
  background-color: #ddf1cf;
  display: flex;
  justify-content: center;
  align-items: center;
}
.first-title {
  margin: 7rem 5rem 0 5rem;
  font-size: 3rem;
}
.second-title {
  color: #ddf1cf;
  margin: 0 5rem 4rem 5rem !important;
  font-size: 3rem;
}
.first-half,
.second-half {
  width: 50%;
  height: 100vh;
}
.layout {
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
}
.paragraph {
  font-size: 1.5rem;
  padding: 0 3rem 0 5rem;
}
.first-title,
.paragraph {
  color: whitesmoke;

  .second-title {
    margin: 0 5rem;
    max-width: 60%;
  }
}
</style>
