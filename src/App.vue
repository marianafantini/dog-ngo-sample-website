<script setup>
import { Layout, ConfigProvider } from 'ant-design-vue';
import ContactUsView from './views/ContactUsView.vue';
import HowWeHelpView from './views/HowWeHelpView.vue';
import HowYouCanHelpView from './views/HowYouCanHelpView.vue';
import AboutView from './views/AboutView.vue';
import HomeView from './views/HomeView.vue';
import MeetLeadersView from './views/MeetLeadersView.vue';
</script>

<template>
  <ConfigProvider
    :theme="{
      token: { fontSize: 24,
        fontFamily: 'Darker Grotesque'},
    }"
  >
    <Layout class="container">
      <div class="slide">
        <HomeView></HomeView>
      </div>
      <div class="slide">
        <AboutView></AboutView>
      </div>
      <div class="slide">
        <HowWeHelpView></HowWeHelpView>
      </div>
      <div class="slide">
        <HowYouCanHelpView></HowYouCanHelpView>
      </div>
      <div class="slide">
        <MeetLeadersView></MeetLeadersView>
      </div>
      <div class="slide">
        <ContactUsView></ContactUsView>
      </div>
    </Layout>
  </ConfigProvider>
</template>

<style scoped>
.container {
  width: 100%;
  height: 100vh;
  overflow-y: scroll;
  scroll-snap-type: y mandatory;
}
.slide {
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 50px;
  scroll-snap-align: start;
}
.header {
  display: flex;
  justify-content: space-between;
  min-height: 5rem;
  background-color: transparent;
}
.content {
  min-height: 70vh;
}
</style>
