<template>
  <div v-swiper="swiperOption" class="swiper-container">
    <div class="swiper-wrapper">
      <div class="swiper-slide">Render original HTML in server, render Swiper in browser (client)</div>
      <div class="swiper-slide">Render original HTML in server, render Swiper in browser (client)</div>
      <div class="swiper-slide">Render original HTML in server, render Swiper in browser (client)</div>
      <div class="swiper-slide">Render original HTML in server, render Swiper in browser (client)</div>
      <div class="swiper-slide">Render original HTML in server, render Swiper in browser (client)</div>
    </div>
    <div class="swiper-pagination"></div>
  </div>
</template>

<script>
import { directive } from "vue-awesome-swiper";
export default {
  directives: {
    swiper: directive
  },
  data() {
    return {
      swiperOption: {
        direction: "vertical",
        mousewheel:true,
        keyboard:true,
        pagination: {
          el: ".swiper-pagination",
          clickable: true
        }
      }
    };
  }
};
</script>
<style scoped>
.swiper-container {
  width: 100%;
  height: 100vh;
}
.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;

  /* Center slide text vertically */
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center;
}
</style>