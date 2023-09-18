<template>
  <div>
    <VueSlickCarousel class="slider">
      <div
        v-for="(slide, idx) in sliderList"
        :key="'slider' + idx"
        class="slide"
      >
        <img :src="slide.img" :alt="slide.img" />
      </div>
    </VueSlickCarousel>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";

export default {
  name: "app-slider",
  components: { VueSlickCarousel },
  data() {
    return {
      settings: {
        dots: true,
        infinite: true,
        slidesToScroll: 1,
        autoplay: true,
        autoplaySpeed: 500,
        pauseOnDotsHover: true,
        pauseOnFocus: true,
        pauseOnHover: true,
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
.slide {
  img {
    object-fit: cover;
  }
}
</style>
