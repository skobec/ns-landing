<template>
  <div class="container__apps">
    <h2 class="title">Скачивай<br>
      прямо сейчас</h2>
    <a href="#" class="app__store__ico">
      <img src="../assets/img/app-store-ico.svg">
    </a>
  </div>
</template>

<script>
export default {
  name: 'app-download-block',
};
</script>

<style scoped lang="scss">
@import "../assets/css/params.scss";

    .container__apps {
      text-align: center;
    }
    .title {
      font-style: normal;
      font-weight: normal;
      font-size: 45px;
      line-height: 90%;
      text-align: center;
      margin-top: 102px;
      margin-bottom: 30px;
    }
@media (max-width: $tablet-size) {
  .title {
    font-style: normal;
    font-weight: normal;
    font-size: 22px;
    line-height: 90%;
    text-align: center;
    margin-top: 43px;
    margin-bottom: 24px;
  }
  .app__store__ico {
    img {
      width: 156px;
    }
  }
}
</style>
