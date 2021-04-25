<template lang="html">
  <div>
    <header-banner/>
    <div class="container">
      <video-instruction/>
      <result-month/>
      <lessons-block/>
      <app-download-block/>
    </div>
    <footer-landing/>
  </div>
</template>

<script>

import HeaderBanner from '../components/header-banner.vue';
import VideoInstruction from '../components/video-instruction.vue';
import ResultMonth from '../components/result-month.vue';
import LessonsBlock from '../components/lessons-block.vue';
import AppDownloadBlock from '../components/app-download-block.vue';
import FooterLanding from '../components/footer.vue';

export default {
  name: 'Index',
  components: {
    FooterLanding,
    AppDownloadBlock,
    LessonsBlock,
    ResultMonth,
    VideoInstruction,
    HeaderBanner,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #ffffff;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #ffffff;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>

