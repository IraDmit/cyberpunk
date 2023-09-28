<template>
  <div class="section">
    <div class="container">
      <div class="leftCol">
        <img
          src="../assets/images/monitor.png"
          alt="monitor"
          class="imgMonitor"
        />
        <div class="logos">
          <img src="../assets/images/hp-logo.svg" alt="logo" class="hp" />
          <img src="../assets/images/x-logo.svg" alt="logo" class="x" />
          <img
            src="../assets/images/Cyberpunk_2077_logo 1.svg"
            alt="logo"
            class="mainLogo"
          />
        </div>
      </div>
      <div class="advertisement">
        <div class="advertisement__text">
          <h2 class="advertisement__text__title">
            Полное погружение вместе с HP
          </h2>
          <div class="advertisement__text__mainInfo">
            Погрузись в современные экшен-игры с реалистичным изображением с
            помощью монитора с диагональю 23,8 дюйма, созданном для отображения
            максимально насыщенных цветов. Успевай реагировать на любые события
            с временем отклика 1 мс и частотой в 144 Гц!
          </div>
          <div class="advertisement__text__list">
            <div class="item">
              <img src="../assets/images/color.svg" alt="icon" />
              <div class="text">Яркие насыщенные цвета</div>
            </div>
            <div class="item">
              <img src="../assets/images/awasome.svg" alt="icon" />
              <div class="text">Кристальная четкость изображения</div>
            </div>
            <div class="item">
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
      .imgMonitor {
        max-width: 100%;
      }
      .logos {
        display: flex;
        gap: 25px;
        margin-top: 26px;
      }
    }
    .advertisement {
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
    @media (max-width: 1024px) {
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
      .advertisement{
        max-width: 50%;
        
      }
    }
  }
}
</style>
