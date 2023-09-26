<template>
  <div class="container">
    <div class="introduce">
      <h2 class="introduce__title">Найт-Сити изменит тебя навсегда!</h2>
      <div class="introduce__text">
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
            src="../assets/images/pic-1.svg"
            alt="picture"
            class="introduce__pictures__item"
          />
          <img
            src="../assets/images/pic-2.svg"
            alt="picture"
            class="introduce__pictures__item"
          />
        </div>
        <div class="rightCol">
          <img
            src="../assets/images/pict-3.svg"
            alt="picture"
            class="introduce__pictures__item"
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
    .leftCol {
      display: flex;
      flex-direction: column;
      gap: 32px;
    }
  }
}
</style>
