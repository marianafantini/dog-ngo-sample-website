<script setup>
import { Layout, Typography } from 'ant-design-vue';
const { Title, Paragraph } = Typography;

const { Content } = Layout;
</script>

<template>
  <Layout class="layout">
    <Content class="content">
      <div class="first-half"></div>
      <div class="second-half">
        <Title :level="2">How You Can Help </Title>
        <Paragraph class="paragraph">
          There are countless ways you can help us in our quest for paws. You can make a donation
          (however big or small), join our fundraiser events, or volunteer your time and home as a
          foster parent.
        </Paragraph>
        <Paragraph class="green-paragraph">⟶ Donate</Paragraph>
        <Paragraph class="green-paragraph">⟶ Join</Paragraph>
        <Paragraph class="green-paragraph">⟶ Volunteer</Paragraph>
      </div>
    </Content>
  </Layout>
</template>

<style lang="scss" scoped>
.content {
  display: flex;
  width: 100%;
}
.second-half {
  background-color: #1c7c54;
}
.first-half {
  background-image: url('../../../public/assets/dog-leash.jpg');
  background-size: 100% auto;
  background-repeat: no-repeat;
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
h2 {
  color: whitesmoke;
  font-size: 4.5rem;
  width: 50%;
  padding: 2.5rem 4rem 0 4rem;
}
.paragraph {
  color: whitesmoke;
}
.paragraph,
.green-paragraph {
  padding: 0 4rem;
  width: 80%;
  font-weight: 500;
}
.green-paragraph {
  color: #ddf1cf;
}
</style>
