<template>
  <div>
    <div class="recommend-title">周末去哪儿?</div>
    <ul>
      <li class="item border-bottom" v-for="item of list" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img"
               :src="item.imgUrl">
        </div>

        <div class="item-info">
          <p class="item-title">{{item.title}} </p>
          <p class="item-desc">{{item.desc}}</p>

        </div>
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    name: 'HomeWeekend',
    props:{
      list:Array
    },
    data() {
      return {
        recommendList: [{
          id: '0001',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1505/86/57819390ea997c.jpg_r_640x214_00888590.jpg',
          title: '郑州打卡',
          desc: '日月轮回，孕育出新的美丽',
          money: '5'
        },
          {
            id: '0002',
            imgUrl: 'http://img1.qunarzz.com/sight/source/1505/86/57819390ea997c.jpg_r_640x214_00888590.jpg',
            title: '少林寺',
            desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
            money: '5'
          },
          {
            id: '0003',
            imgUrl: 'http://img1.qunarzz.com/sight/source/1505/86/57819390ea997c.jpg_r_640x214_00888590.jpg',
            title: '少林寺',
            desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
            money: '5'
          },
          {
            id: '0004',
            imgUrl: 'http://img1.qunarzz.com/sight/source/1505/86/57819390ea997c.jpg_r_640x214_00888590.jpg',
            title: '少林寺',
            desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
            money: '5'
          },
          {
            id: '0005',
            imgUrl: 'http://img1.qunarzz.com/sight/source/1505/86/57819390ea997c.jpg_r_640x214_00888590.jpg',
            title: '少林寺',
            desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
            money: '5'
          }, {
            id: '0006',
            imgUrl: 'http://img1.qunarzz.com/sight/source/1505/86/57819390ea997c.jpg_r_640x214_00888590.jpg',
            title: '少林寺',
            desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
            money: '5'
          }, {
            id: '0007',
            imgUrl: 'http://img1.qunarzz.com/sight/source/1505/86/57819390ea997c.jpg_r_640x214_00888590.jpg',
            title: '少林寺',
            desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
            money: '5'
          }
        ]
      };
    }
  };


</script>

<style lang="stylus" scoped>
  .recommend-title
    line-height: .8rem;
    background: #eee;
    text-indent: .2rem
    margin-top: .2rem

  .item-img-wrapper
    overflow: hidden
    height: 0
    padding-bottom: 37.4375%

    .item-img
      width: 100%

  .item-info
    padding: .14rem .2rem .2rem .2rem
    min-width: 0;

  .item-title
    line-height: .48rem
    font-size: .28rem
    color: #212121
    padding-right: 1.4rem
    overflow: hidden
    white-space: nowrap;
    text-overflow: ellipsis

  .item-desc
    line-height: .42rem;
    font-size: .24rem
    color: #616161
    overflow: hidden
    white-space: nowrap;
    text-overflow: ellipsis;
    padding-right: 1.4rem
</style>
