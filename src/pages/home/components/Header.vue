<template>
    <div class="header">
        <div class="header-left">
            <div class="iconfont back-icon">&#xeb99;</div>
        </div>
        <div class="header-input">
            <span class="iconfont">&#xeb9c;</span>
            输入城市/景点/游玩/主题
        </div>
        <div class="header-right ">
            城市
            <span class="iconfont arrow-icon">&#xe64a;</span>
        </div>
    </div>

</template>

<script>
  import {style} from '../../../assets/styles/varibles';

  console.log(style['theme-color']);
  export default {
    name: 'HomeHeader'
  };
</script>

<style lang="stylus" scoped>
    .header
        display: flex
        height: 0.86rem;
        background: #00bcd4;
        color: #ffffff;
        line-height: 0.86rem;

        .header-left
            width: 0.64rem;
            float: left;

            .back-icon {
                text-align: center;
                font-size: 0.4rem;
            }

        .header-input
            flex: 1;
            background: #ffffff;
            border-radius: 0.1rem;
            line-height: 0.64rem;
            height: 0.64rem;
            margin-top: 0.12rem;
            margin-left 0.2rem;
            color: #ccc
            padding-left: 0.1rem


        .header-right
            width: 1.24rem;
            float: right;
            text-align: center

            .arrow-icon {
                font-size: 0.23rem;
                margin-left: -0.04rem;
            }


</style>
