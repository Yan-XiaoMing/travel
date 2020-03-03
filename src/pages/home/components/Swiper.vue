<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <swiper-slide v-for="item of swiperList" :key="item.id">
                <img class="swiper-img" :src="item.imgUrl"/>
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
              pagination: '.swiper-pagination',
              loop: true
          },
          swiperList: [{
              id: '0001',
              imgUrl: 'http://img.alicdn.com/imgextra/i2/144/O1CN015RWsBW1CvzcUfWItz_!!144-0-luban.jpg'
          }, {
              id: '0002',
              imgUrl: 'http://img.alicdn.com/imgextra/i2/144/O1CN015RWsBW1CvzcUfWItz_!!144-0-luban.jpg'
          }]
      };
    }
  };
</script>

<style lang="stylus" scoped>
    .wrapper >>> .swiper-pagination-bullet-active
        background: #fff
    .wrapper
        overflow: hidden;
        width: 100%;
        height: 0
        padding-bottom: 31%;
        background: grey;

        .swiper-pagination
            color: #ffffff
            bottom: -1rem
            width: 1rem;
            height: 1rem

    img
        width: 100%;

</style>
