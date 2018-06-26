<template>
<div class="wrapper">
    <swiper :options="swiperOption">
        <!-- slides -->
        <swiper-slide>
            <img src="https://img1.qunarzz.com/order/comp/1805/2e/6e407f088bfb902.png" alt="slide 1" class="swiper-image">
        </swiper-slide>
        <swiper-slide>        
            <img src="https://img1.qunarzz.com/order/comp/1805/2e/6e407f088bfb902.png" alt="slide 2" class="swiper-image">
        </swiper-slide>
        <!-- Optional controls -->
        <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
</div>

</template>

<script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      swiperOption: {
          pagination: ".swiper-pagination"
      }
    };
  }
};
</script>

<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active
    background: #fff !important 

.wrapper
    width: 100%
    height: 31.25vw
    background: #eee
    .swiper-image
        width: 100%

</style>
