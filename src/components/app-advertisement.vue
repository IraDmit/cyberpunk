<template>
  <div class="section">
    <div class="container">
      <div class="leftCol">
        <img
          src="../assets/images/monitor.png"
          alt="monitor"
          class="imgMonitor wow fadeInLeftBig"
          data-wow-duration="1.5s"
        />
        <div class="logos">
          <img
            src="../assets/images/hp-logo.svg"
            alt="logo"
            class="hp wow fadeInLeftBig"
            data-wow-duration="1.5s"
            data-wow-delay="1s"
          />
          <img
            src="../assets/images/x-logo.svg"
            alt="logo"
            class="x wow fadeInLeftBig"
            data-wow-duration="1.5s"
            data-wow-delay="0.7s"
          />
          <img
            src="../assets/images/Cyberpunk_2077_logo 1.svg"
            alt="logo"
            class="mainLogo wow fadeInLeftBig"
            data-wow-duration="1.5s"
            data-wow-delay="0.5s"
          />
        </div>
      </div>
      <div class="advertisement">
        <div class="advertisement__text">
          <h2 class="advertisement__text__title wow fadeInRightBig">
            Полное погружение вместе с HP
          </h2>
          <div class="advertisement__text__mainInfo wow fadeInRightBig" data-wow-delay="0.5s">
            Погрузись в современные экшен-игры с реалистичным изображением с
            помощью монитора с диагональю 23,8 дюйма, созданном для отображения
            максимально насыщенных цветов. Успевай реагировать на любые события
            с временем отклика 1 мс и частотой в 144 Гц!
          </div>
          <div class="advertisement__text__list">
            <div class="item wow fadeInRightBig" data-wow-delay="1s">
              <img src="../assets/images/color.svg" alt="icon" />
              <div class="text">Яркие насыщенные цвета</div>
            </div>
            <div class="item wow fadeInRightBig" data-wow-delay="1.3s">
              <img src="../assets/images/awasome.svg" alt="icon" />
              <div class="text">Кристальная четкость изображения</div>
            </div>
            <div class="item wow fadeInRightBig" data-wow-delay="1.6s">
              <img src="../assets/images/motion.svg" alt="icon" />
              <div class="text">Быстрые движения и плавный геймплей</div>
            </div>
          </div>
          <div class="advertisement__text__btn">Подробнее</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.wow {
  visibility: hidden;
}
.section {
  background-color: #f8f200;
  .container {
    padding: 70px 30px;
    display: flex;
    gap: 32px;
    .leftCol {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      width: calc(50% - 32px);
      .imgMonitor {
        max-width: 100%;
      }
      .logos {
        display: flex;
        gap: 25px;
        margin-top: 26px;
        img {
          height: unset;
        }
      }
    }
    .advertisement {
      width: calc(50% - 32px);
      &__text {
        &__title {
          color: #000;
          font-family: Archangelsk;
          font-size: 62px;
          font-style: normal;
          font-weight: 400;
          line-height: normal;
          margin: 0;
        }
        &__mainInfo {
          color: #000;
          font-family: Roboto;
          font-size: 18px;
          font-style: normal;
          font-weight: 400;
          line-height: 34px;
          margin: 25px 0;
        }
        &__list {
          display: flex;
          flex-direction: column;
          gap: 15px;
          .item {
            display: flex;
            gap: 10px;
            align-items: center;
            color: #000;
            font-family: Roboto;
            font-size: 18px;
            font-style: normal;
            font-weight: 400;
            line-height: normal;
          }
        }
        &__btn {
          color: #f8f200;
          font-family: Roboto;
          font-size: 18px;
          font-style: normal;
          font-weight: 700;
          line-height: normal;
          display: inline-flex;
          background-color: #000;
          padding: 15px 50px;
          align-items: center;
          margin-top: 40px;
          cursor: pointer;
        }
      }
    }
    @media (max-width: 1124px) {
      .leftCol .logos {
        flex-direction: column;
        align-items: center;
        max-width: 50%;
        width: 100%;
        .hp {
          width: 80px;
          height: 80px;
        }
        .x {
          height: 19.183px;
          width: 90px;
        }
      }
      .advertisement {
        max-width: 50%;
      }
    }
    @media (max-width: 700px) {
      flex-direction: column;
      .advertisement {
        max-width: 100%;
      }
    }
    @media (max-width: 500px) {
      .advertisement__text__title {
        font-size: 30px;
      }
    }
  }
}
</style>
