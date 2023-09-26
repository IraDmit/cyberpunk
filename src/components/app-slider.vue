<template>
  <div class="slider-content">
    <VueSlickCarousel class="slider" v-bind="settings">
      <div
        v-for="(slide, idx) in sliderList"
        :key="'slider' + idx"
        class="slide"
      >
        <img :src="slide.img" :alt="slide.img" />
      </div>
    </VueSlickCarousel>
    <div class="container">
      <div class="more-info">
        <h2 class="more-info__title">Доступно на всех платформах</h2>
        <div class="more-info__btn">Узнать больше</div>
      </div>
    </div>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";

export default {
  name: "app-slider",
  components: { VueSlickCarousel },
  data() {
    return {
      settings: {
        arrows: false,
        dots: false,
        infinite: true,
        slidesToScroll: 1,
        autoplay: true,
        autoplaySpeed: 5000,
        pauseOnFocus: true,
        fade: true,
      },
      sliderList: [
        {
          img: require("../assets/images/11.jpg"),
        },
        {
          img: require("../assets/images/12.jpg"),
        },
        {
          img: require("../assets/images/Untitled-1 2.jpg"),
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
h2 {
  margin: 0;
}

.slider-content {
  position: relative;
  height: 100vh;
  .slider {
    width: 100%;
    height: 100%;
    .slick-list {
      height: 100%;
    }
    .slick-track {
      height: 100vh;
    }
    .slide {
      img {
        max-width: 100%;
      }
    }
  }
  .container {
    position: relative;
    .more-info {
      position: absolute;
      bottom: 0;
      right: 0;
      background-color: #f8f200;
      max-width: 624px;
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
      padding: 70px;
      &__title {
        font-family: Archangelsk;
        font-size: 62px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
      }
      &__btn {
        cursor: pointer;
        display: inline-flex;
        padding: 19px 50px;
        align-items: center;
        background-color: #000;
        color: #f8f200;
        text-align: center;
        font-family: Roboto;
        font-size: 24px;
        font-style: normal;
        font-weight: 700;
        line-height: 40px;
        margin-top: 25px;
      }
    }
  }
}
</style>
