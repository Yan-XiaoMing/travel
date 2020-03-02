<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <swiper-slide>
                <img src="https://dimg04.c-ctrip.com/images/zg0u1c000001e40okDCDB.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="https://dimg04.c-ctrip.com/images/zg0u1c000001e40okDCDB.jpg"/>
            </swiper-slide>
            <!-- Optional controls -->
            <div class="swiper-pagination" slot="pagination"></div>
        </swiper>
    </div>


</template>

<script>
  export default {
    name: 'HomeSwiper',
    data() {
      return {
        swiperOption: {
          pagination: '.swiper-pagination'
        }
      };
    }
  };
</script>

<style lang="stylus" scoped>
    .wrapper >>> .swiper-pagination-bullet-active
        background: white

    .wrapper
        overflow: hidden;
        width: 100%;
        height: 0
        padding-bottom: 60%;
        background: grey

    img
        width: 100%;

</style>
