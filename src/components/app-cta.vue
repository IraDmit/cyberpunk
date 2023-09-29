<template>
  <div class="cta">
    <div class="container">
      <div class="first-row">
        <div class="cta__title">
          <img
            src="../assets/images/Group215sale.png"
            alt="sale"
            class="cta__title__logoSale"
          />

          <h2 class="cta__title__text">Играй и выигрывай!</h2>
        </div>
        <div class="cta__text">
          Играй в <span> Cyberpunk 2077</span> и получи возможность выиграть
          консоль <span> Xbox Series X</span> или
          <span> Sony PlayStation 5!</span> Заполни форму ниже и приложи
          скриншот о покупке игры. Итоги розыгрыша будут подведены 1 февраля.
          Удачи! ;)
        </div>
      </div>

      <div class="cta__leftCol">
        <div class="cta__leftCol__form">
          <input
            type="text"
            placeholder="Как тебя зовут?"
            class="custom-input"
          />
          <input type="text" placeholder="Твой е-mail" class="custom-input" />
          <input type="file" id="file" class="file-input" />
          <label for="file" class="custom-input-file">
            <span>Прикрепить скриншот</span>
            <span class="format">.png / .jpg / .pdf</span>
          </label>
          <div class="btn">Отправить</div>
          <div class="checkbox-wrp">
            <div
              class="checkbox"
              @click="checkbox = !checkbox"
              :class="{ active: checkbox }"
            ></div>
            <span @click="checkbox = !checkbox"
              >Согласен на обработку персональных данных</span
            >
          </div>
        </div>
      </div>
      <div class="cta__rightCol">
        <picture>
          <source media="(max-width: 880px)" srcset="../assets/images/ps.svg" />
          <source
            media="(max-width: 1350px)"
            srcset="../assets/images/Group244vertical.png"
          />
          <img src="../assets/images/ps.svg" alt="" />
        </picture>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      checkbox: true,
    };
  },
};
</script>

<style lang="scss" scoped>
.cta {
  position: relative;
  background-color: #000;
  height: 100vh;
  padding: 70px 0;
  // display: flex;
  gap: 32px;
  width: 100%;
  &::after {
    position: absolute;
    content: "";
    background-image: url("../assets/images/bg-yellow-black.png");
    bottom: 0;
    left: 0;
    width: 100%;
    height: 70px;
  }
  &::before {
    position: absolute;
    content: "";
    background-image: url("../assets/images/bg-white-black.png");
    top: 0;
    left: 0;
    width: 100%;
    height: 70px;
  }
  .container {
    display: grid;
    grid-template-columns: 460px 788px;
    grid-gap: 25px;
    .first-row {
      grid-column: 1 / span 2;
    }
  }
  &__title {
    gap: 32px;
    display: flex;
    margin-bottom: 39px;
    &__logoSale {
      max-width: 132px;
    }
    &__text {
      align-self: flex-end;
      color: #fff;
      font-family: Archangelsk;
      font-size: 62px;
      font-style: normal;
      font-weight: 400;
      line-height: normal;
      margin: 0;
    }
  }
  &__text {
    color: #fff;
    font-family: Roboto;
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: 34px;
    max-width: 952px;
    span {
      color: #52bedc;
      font-weight: 700;
    }
  }

  &__leftCol {
    margin-top: 66px;
    margin-right: 32px;
    &__form {
      display: flex;
      flex-direction: column;
      .custom-input {
        border: none;
        outline: none;
        padding: 0 0 13px 0;
        background-color: unset;
        border-bottom: 1px solid #777;
        color: #fff;
        margin-bottom: 35px;
        &::placeholder {
          color: #fff;
          font-family: Roboto;
          font-size: 18px;
          font-style: normal;
          font-weight: 300;
          line-height: normal;
        }
      }
      .file-input {
        display: none;
      }
      .custom-input-file {
        margin-bottom: 35px;
        border: 1px dashed #777;
        padding: 39px 130px;
        cursor: pointer;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 7px;
        span {
          color: #fff;
          font-family: Roboto;
          font-size: 18px;
          font-style: normal;
          font-weight: 300;
          line-height: normal;
          text-decoration-line: underline;
        }
        .format {
          font-size: 12px;
          text-decoration: none;
        }
      }
      .btn {
        display: inline-flex;
        height: 59px;
        padding: 15px 50px;
        align-items: center;
        flex-shrink: 0;
        background: #f8f200;
        color: #000;
        font-family: Roboto;
        font-size: 18px;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
        max-width: 192px;
        cursor: pointer;
        margin-bottom: 12px;
      }
      .checkbox-wrp {
        display: flex;
        cursor: pointer;
        .checkbox {
          width: 14px;
          height: 14px;
          border: 1px solid #777;

          &.active {
            background-image: url("../assets/images/ok.svg");
          }
        }
        span {
          color: #fff;
          font-family: Roboto;
          font-size: 12px;
          font-style: normal;
          font-weight: 300;
          line-height: normal;
          margin-left: 10px;
        }
      }
    }
  }
  &__rightCol {
    width: 100%;
    img {
      max-width: 100%;
    }
  }
  @media (max-width: 1350px) {
    height: auto;
    .container {
      grid-template-columns: 1fr 1fr;
      .first-row {
        grid-column: unset;
      }
      .cta__rightCol {
        grid-row: 1 / span 2;
      }
    }
  }
  @media (max-width: 880px) {
    .container {
      grid-template-columns: 1fr;
      .cta__leftCol {
        margin-right: 0;
      }
      .cta__rightCol {
        grid-row: unset;
        order: -2;
        img {
          width: 100%;
        }
      }
    }
  }
  @media (max-width: 600px) {
    .cta__leftCol__form {
      .custom-input-file {
        padding: 30px 0;
      }
    }
    .cta__title {
      position: relative;
      &__logoSale {
        position: absolute;
        left: -9%;
        top: -250%;
      }
    }
  }
  @media (max-width: 500px) {
    .cta__title__text {
      font-size: 30px;
    }
  }
}
</style>
