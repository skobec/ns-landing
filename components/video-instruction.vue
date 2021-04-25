<template lang="html">
  <div class="video__block__container">
    <h2 class="title">Как работает сервис</h2>
    <div class="video__block">
      <iframe width="100%" height="100%" src="https://www.youtube-nocookie.com/embed/Jiz5MJneVmY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
  </div>
</template>

<script>
export default {
  name: 'videoInstruction',
};
</script>

<style scoped lang="scss">
@import "../assets/css/params.scss";

  .video__block__container {
    margin-bottom: 97px;
  }
  .title {
    font-style: normal;
    font-weight: normal;
    font-size: 45px;
    line-height: 90%;
    text-align: center;
    margin-bottom: 45px;
  }
  .video__block {
    max-width: 800px;
    height: 480px;
    background: #C4C4C4;
    border-radius: 8px;
    margin: 0 auto;
    overflow: hidden;
  }

@media (max-width: $tablet-size) {
  .video__block__container {
    margin-bottom: 38px;
  }
  .title {
    font-style: normal;
    font-weight: normal;
    font-size: 24px;
    line-height: 28px;
    text-align: center;
    margin-top: 38px;
    margin-bottom: 30px;
  }
  .video__block {
    height: 255px;
  }
}

@media (max-width: $mobile-size) {
  .video__block {
    height: 174px;
  }
}
</style>
