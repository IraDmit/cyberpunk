<template>
  <div class="container">
    <div class="introduce">
      <h2 class="introduce__title wow fadeInDown" data-wow-duration="2s">Найт-Сити изменит тебя навсегда!</h2>
      <div class="introduce__text wow fadeInDown" data-wow-duration="2.5s">
        <span> Cyberpunk 2077 </span>— приключенческая ролевая игра, действие
        которой происходит в мегаполисе Найт-Сити, где власть, роскошь и
        модификации тела ценятся выше всего. Ты играешь за V, наёмника в поисках
        устройства, позволяющего обрести бессмертие. Ты сможешь менять
        киберимпланты, навыки и стиль игры своего персонажа, исследуя открытый
        мир, где твои поступки влияют на ход сюжета и всё, что тебя окружает.
      </div>
      <div class="introduce__pictures">
        <div class="leftCol">
          <img
            src="../assets/images/pic-3.png"
            alt="picture"
            class="introduce__pictures__item wow slideInLeft"
            data-wow-duration="2s"
          />
          <img
            src="../assets/images/pic-2.png"
            alt="picture"
            class="introduce__pictures__item wow slideInLeft"
            data-wow-duration="2s"
          />
        </div>
        <div class="rightCol">
          <img
            src="../assets/images/pic-1.png"
            alt="picture"
            class="introduce__pictures__item wow fadeInRightBig"
            data-wow-duration="2s"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  margin-top: 140px;
}
.introduce {
  margin: 70px 0;
  &__title {
    font-family: Archangelsk;
    font-size: 62px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    margin: 0 0 25px 0;
  }
  &__text {
    font-family: Roboto;
    font-size: 18px;
    font-style: normal;
    font-weight: 700;
    line-height: 34px;
    color: #777;
    max-width: 952px;
    margin-bottom: 70px;
    span {
      color: #52bedc;
    }
  }
  &__pictures {
    display: grid;
    grid-template-columns: 1fr 2fr;
    gap: 32px;
    // height: 788px;
    // overflow: hidden;
    .leftCol {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      img {
        // height: 196px;
        max-width: 460px;
        width: 100%;
        -webkit-clip-path: polygon(
          7% 0,
          100% 0,
          100% 87%,
          93% 100%,
          0 100%,
          0% 60%,
          0 13%
        );
        clip-path: polygon(
          7% 0,
          100% 0,
          100% 87%,
          93% 100%,
          0 100%,
          0% 60%,
          0 13%
        );
      }
    }
    .rightCol {
      // height: 424px;
      overflow: hidden;
      -webkit-clip-path: polygon(
        7% 0,
        100% 0,
        100% 87%,
        93% 100%,
        0 100%,
        0% 60%,
        0 13%
      );
      clip-path: polygon(
        7% 0,
        100% 0,
        100% 87%,
        93% 100%,
        0 100%,
        0% 60%,
        0 13%
      );
      img {
        -webkit-clip-path: polygon(
          7% 0,
          100% 0,
          100% 87%,
          93% 100%,
          0 100%,
          0% 60%,
          0 13%
        );
        clip-path: polygon(
          7% 0,
          100% 0,
          100% 87%,
          93% 100%,
          0 100%,
          0% 60%,
          0 13%
        );
        max-width: 788px;
      }
    }
  }
  @media (max-width: 1024px) {
    &__pictures {
      grid-template-columns: 1fr;
      .leftCol {
        flex-direction: row;
        justify-content: space-between;
        img {
          max-width: calc(50% - 16px);
        }
      }
      .rightCol {
        img {
          max-width: 952px;
          width: 100%;
        }
      }
    }
  }
  @media (max-width: 623px) {
    margin-top: 300px;

    &__text {
      font-size: 16px;
    }
    &__pictures {
      grid-template-columns: 1fr;
      .leftCol {
        flex-direction: column;
        justify-content: space-between;
        gap: 35px;
        img {
          max-width: 100%;
          width: 100%;
        }
      }
      .rightCol {
        img {
          max-width: 100%;
          width: 100%;
          height: auto;
        }
      }
    }
  }
  @media (max-width: 500px) {
    &__title {
      font-size: 30px;
    }
  }
}
</style>
