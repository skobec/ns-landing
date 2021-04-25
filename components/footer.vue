<template>
  <div class="footer">
    <div class="container">
      <div class="links__block">
        <a href="#" class="link">Политика конфиденциальности</a>
        <a href="#" class="link">Пользовательское соглашение</a>
      </div>
      <div class="soc__ico">
        <a href="#" class="insta soc__btn">
          <img src="../assets/img/insta.svg">
        </a>
        <a href="#" class="telegram soc__btn">
          <img src="../assets/img/telegram.svg">
        </a>
      </div>
      <p class="copyright">Copyright 2021 Все права защищены</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'footerLanding',
};
</script>

<style scoped lang="scss">
@import "../assets/css/params.scss";

  .footer {
    margin-top: 45px;
    border-top: 1px solid #373737;
    text-align: center;
    padding-top: 17px;
    padding-bottom: 146px;
    &* {
      color: #707070;
    }
    .links__block {
      display: flex;
      justify-content: space-evenly;
      margin-bottom: 26px;
    }
    .link {
      color: #707070;
    }
    .copyright {
      margin-top: 26px;
      display: inline-flex;
    }
    .soc__ico {
      display: flex;
      text-align: center;
      justify-content: center;
    }
    .soc__btn {
      width: 42px;
      height: 42px;
      border-radius: 50%;
      background-color: #58595C;
      display: flex;
      align-items: center;
      margin: 0 7px;
      img {
        margin: 0 auto;
      }
    }
  }

@media (max-width: $tablet-size) {
  .footer {
    padding-bottom: 22px;
    margin: 56px 15px 0;
    .links__block {
      flex-direction: column;
    }
    .link {
      font-style: normal;
      font-weight: normal;
      font-size: 11px;
      line-height: 150%;
      text-align: center;
      margin-bottom: 9px;
    }
    .copyright {
      font-style: normal;
      font-weight: normal;
      font-size: 11px;
      line-height: 150%;
    }
    .soc__btn {
      width: 32px;
      height: 32px;
      img {
        width: 16px;
      }
    }
  }
}
</style>
