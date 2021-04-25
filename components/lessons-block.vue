<template lang="html">
  <div class="lesson__container">
    <h2 class="title">Получи 10 уроков <br>по инвестициям</h2>
    <div class="container__lessons">
      <a href="#" class="lessons__item">
        <div class="preview">
          <img src="../assets/img/lessons/less1.png">
        </div>
        <div class="text">
          <p class="title__less">Урок 1</p>
          <p class="desc">Как и зачем начинать инвестировать?</p>
        </div>
      </a>
      <a href="#" class="lessons__item">
        <div class="preview">
          <img src="../assets/img/lessons/less1.png">
        </div>
        <div class="text">
          <p class="title__less">Урок 2</p>
          <p class="desc">Как правильно использовать
            сигналы и извлекать из этого максимальную прибыль?</p>
        </div>
      </a>
      <a href="#" class="lessons__item">
        <div class="preview">
          <img src="../assets/img/lessons/less1.png">
        </div>
        <div class="text">
          <p class="title__less">Урок 3</p>
          <p class="desc">У какого брокера открыть счёт?</p>
        </div>
      </a>
      <a href="#" class="lessons__item">
        <div class="preview">
          <img src="../assets/img/lessons/less1.png">
        </div>
        <div class="text">
          <p class="title__less">Урок 4</p>
          <p class="desc">9 ресурсов по отбору акций в свой портфель</p>
        </div>
      </a>
      <a href="#" class="lessons__item">
        <div class="preview">
          <img src="../assets/img/lessons/less1.png">
        </div>
        <div class="text">
          <p class="title__less">Урок 5</p>
          <p class="desc">Как из 8000 акций отобрать 10 перспективных в свой портфель?</p>
        </div>
      </a>
      <a href="#" class="lessons__item">
        <div class="preview">
          <img src="../assets/img/lessons/less1.png">
        </div>
        <div class="text">
          <p class="title__less">Урок 6</p>
          <p class="desc">Как я делаю 60% годовых на фондовом рынке?</p>
        </div>
      </a>
      <a href="#" class="lessons__item">
        <div class="preview">
          <img src="../assets/img/lessons/less1.png">
        </div>
        <div class="text">
          <p class="title__less">Урок 7</p>
          <p class="desc">Построение своей стратегии инвестирования</p>
        </div>
      </a>
      <a href="#" class="lessons__item">
        <div class="preview">
          <img src="../assets/img/lessons/less1.png">
        </div>
        <div class="text">
          <p class="title__less">Урок 8</p>
          <p class="desc">6 бесплатных источников по развитию навыков инвестирования</p>
        </div>
      </a>
      <a href="#" class="lessons__item">
        <div class="preview">
          <img src="../assets/img/lessons/less1.png">
        </div>
        <div class="text">
          <p class="title__less">Урок 9</p>
          <p class="desc">10 способов потерять деньги на фондовом рынке</p>
        </div>
      </a>
      <a href="#" class="lessons__item">
        <div class="preview">
          <img src="../assets/img/lessons/less1.png">
        </div>
        <div class="text">
          <p class="title__less">Урок 10</p>
          <p class="desc">Как я управляю 1 миллионном,
            который мне дал популярный блогер Михаил Литвин?</p>
        </div>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'LessonsBlock',
};
</script>

<style scoped lang="scss">
@import "../assets/css/params.scss";

  .lesson__container {
    margin-top: 90px;
  }
  .title {
    font-style: normal;
    font-weight: normal;
    font-size: 45px;
    line-height: 90%;
    text-align: center;
    margin-bottom: 68px;
  }

  .container__lessons {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 42px;
  }
  .lessons__item {
    display: flex;
    text-align: left;
    align-items: center;
    .preview {
      flex-basis: 122.86px;
      height: 82.86px;
      border-radius: 6px;
      overflow: hidden;
      margin-right: 20px;
      img {
        width: 100%;
        border-radius: 6px;
      }
    }
    .text {
      flex-basis: 220px;
      .title__less {
        font-style: normal;
        font-weight: bold;
        font-size: 13px;
        line-height: 15px;
        text-transform: uppercase;
        color: #0177FD;
      }
      .desc {
        margin-top: 3px;
        font-style: normal;
        font-weight: normal;
        font-size: 14px;
        line-height: 16px;
        color: #FFFFFF;
        margin-bottom: 0;
      }
    }
  }

@media (max-width: $tablet-size) {
  .title {
    font-style: normal;
    font-weight: normal;
    font-size: 24px;
    line-height: 28px;
    text-align: center;
    margin-top: 38px;
    margin-bottom: 30px;
  }
  .lesson__container {
    margin-top: 50px;
  }
  .container__lessons {
    grid-template-columns: 1fr;
    grid-gap: 15px;
  }
  .lessons__item {
    align-items: start;
    .preview {
      height: 56px;
      flex-basis: 83px;
      margin-right: 15px;
    }
    .title__less {
      font-style: normal;
      font-weight: bold;
      font-size: 11px;
      line-height: 13px;
      text-transform: uppercase;
      margin-bottom: 4px;
      margin-top: 0;
    }
    .desc {
      font-style: normal;
      font-weight: normal;
      font-size: 12px;
      line-height: 14px;
    }
  }
}
</style>
