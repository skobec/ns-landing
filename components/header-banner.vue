<template lang="html">
  <div>
    <div class="container__banner">
      <div class="header">
        <div class="logo"></div>
      </div>
      <div class="mobile__container">
        <div class="mobile__content">
          <h1 class="title">Получай ежедневные сигналы рынка акций</h1>
          <div class="mobile__image">
            <img src="~/assets/img/mobile-image.png"/>
          </div>
          <a href="#" class="app__store__ico">
            <img src="~/assets/img/app-store-ico.svg">
          </a>
        </div>
        <div class="mobile__image">
          <img src="~/assets/img/mobile-image.png"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'header-banner',
};
</script>

<style scoped lang="scss">
@import "../assets/css/params.scss";
  .mobile__container {
    display: flex;
    align-items: center;
  }

  .title {
    font-style: normal;
    font-weight: normal;
    font-size: 47px;
    line-height: 55px;
    text-align: left;
    margin: 0 0 70px;
  }

  .mobile__image {
    width: 50%;
  }
  .container__banner {
    padding-top: 40px;
    margin: 0 auto 48px;
    max-width: 1100px;
    &:before {
      content: "";
      position: absolute;
      width: 749.2px;
      height: 541.72px;
      background: #FFFFFF;
      opacity: 0.1;
      filter: blur(116px);
      transform: rotate(-28.08deg);
      top: -60%;
      left: 0;
      right: 0;
      margin: auto;
    }
  }
  .logo {
    width: 45px;
    height: 45px;
    left: 120px;
    background: #3D3E44 url("../assets/img/K-logo.svg")no-repeat bottom left;
    background-size: 25px 26px;
    border-radius: 5px;
  }

  .mobile__content {
    .mobile__image {
      display: none;
    }
  }

  @media (max-width: $tablet-size){
    .container__banner {
      padding: 12px 15px 0;
      &:before {
        width: 60%;
        top: -35%;
        transform: none
      }
    }
    .logo {
      margin: 0 auto;
    }
    .title {
      font-style: normal;
      font-weight: normal;
      font-size: 24px;
      line-height: 28px;
      text-align: center;
      margin-top: 14px;
      margin-bottom: 18px;
    }
    .mobile__container {
      flex-direction: column;
    }
    .mobile__content {
      text-align: center;
      .mobile__image {
        display: inline-block;
        width: 100%;
        overflow: hidden;
        img {
          width: 100%;
          margin-left: 40px;
        }
      }
    }
    .mobile__image {
      display: none;
    }
  }
</style>
