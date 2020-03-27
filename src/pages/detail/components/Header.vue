<template>
  <div>
    <router-link tag="div" to="/" class="header-abs">
      <div class="iconfont header-abs-back">&#xeb99;</div>
    </router-link>
    <div class="header-fixed"></div>
  </div>

</template>

<script>
  export default {
    name: 'DetailHeader',
    components: {},
    data() {
      return {
        showGallery: false,
        imgs: ['http://img1.qunarzz.com/sight/p0/1801/ad/ad7b65ceb7a8420ea3.img.jpg_r_800x800_8e9eceda.jpg',
          'http://img1.qunarzz.com/sight/p0/1801/24/24ff8c2d2c495b4ca3.img.jpg_r_800x800_01b9bdd2.jpg']
      };
    },
    methods: {
      handleBannerClick() {
        this.showGallery = true;
      },
      handleGalleryClose() {
        this.showGallery = false;
      }
    }
  };
</script>

<style scoped lang="stylus">
  .header-abs
    position: absolute
    left: .2rem
    top: .2rem
    width: .8rem
    height: .8rem
    border-radius: .4rem
    text-align: center
    line-height: .8rem
    background: rgba(0, 0, 0, 0.8)

    .header-abs-back
      color: #fff
      font-size: .4rem

</style>
<!--.header-fixed-->
<!--position :relative-->
<!--overflow : hidden-->
<!--text-align :center-->
<!--height : .86rem-->
<!--line-height : .86rem-->
<!--color : white-->
<!--background : #00bcd4-->
<!--font-size: .32rem-->
<!--.header-back{-->
<!--position : absolute-->
<!--top :0-->
<!--left : 0-->
<!--width : .64rem-->
<!--text-align :center-->
<!--font-size : .4rem-->
<!--color :#ffffff-->
