<template>
  <div class="cta">
    <div class="container">
      <div class="cta__title">
        <div class="cta__title__logoSale">
          <img src="../assets/images/sale.svg" alt="sale" />
          <span>акция</span>
        </div>
        <h2 class="cta__title__text">Играй и выигрывай!</h2>
      </div>
      <div class="cta__text">
        Играй в <span> Cyberpunk 2077</span> и получи возможность выиграть
        консоль <span> Xbox Series X</span> или
        <span> Sony PlayStation 5!</span> Заполни форму ниже и приложи скриншот
        о покупке игры. Итоги розыгрыша будут подведены 1 февраля. Удачи! ;)
      </div>
      <div class="cta__main">
        <div class="cta__main__leftCol">
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
        <div class="cta__main__rightCol">
          <img src="../assets/images/ps.svg" alt="" />
        </div>
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
  &__title {
    gap: 32px;
    display: flex;
    margin-bottom: 39px;
    &__logoSale {
      position: relative;
      img {
        width: 100%;
      }
      span {
        transform: rotate(-45deg);
        position: absolute;
        top: 36%;
        left: 22%;
        color: #f8f200;
        font-family: Archangelsk;
        font-size: 30px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
      }
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
  &__main {
    display: flex;
    gap: 32px;
    &__leftCol {
      margin-top: 98px;
      display: flex;
      flex-direction: column;
      gap: 35px;
      .custom-input {
        border: none;
        outline: none;
        padding: 0 0 13px 0;
        background-color: unset;
        border-bottom: 1px solid #777;
        color: #fff;
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
    &__rightCol {
    }
  }
}
</style>
