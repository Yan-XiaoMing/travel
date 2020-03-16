<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul>

      <router-link tag="li" class="item border-bottom" v-for="item of list" :key="item.id" :to="'/detail/'+item.id">
        <img class="item-img"
             :src="item.imgUrl">
        <div class="item-info">
          <p class="item-title">{{item.title}} </p>
          <p class="item-desc">{{item.desc}}</p>
          <div class="item-end">
            <span class="item-money">￥{{item.money}}</span>
            <button class="item-button">查看详情</button>
          </div>
        </div>
      </router-link>

    </ul>
  </div>
</template>

<script>
  export default {
    name: 'HomeRecommend',
    props: {
      list: Array
    },
    data() {
      return {
        recommendList: [{
          id: '0001',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1709/e9/e9b7ae23f567806ea3.img.jpg_256x160_659f7c33.jpg',
          title: '少林寺',
          desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
          money: '5'
        },
          {
            id: '0002',
            imgUrl: 'http://img1.qunarzz.com/sight/p0/1709/e9/e9b7ae23f567806ea3.img.jpg_256x160_659f7c33.jpg',
            title: '少林寺',
            desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
            money: '5'
          },
          {
            id: '0003',
            imgUrl: 'http://img1.qunarzz.com/sight/p0/1709/e9/e9b7ae23f567806ea3.img.jpg_256x160_659f7c33.jpg',
            title: '少林寺',
            desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
            money: '5'
          },
          {
            id: '0004',
            imgUrl: 'http://img1.qunarzz.com/sight/p0/1709/e9/e9b7ae23f567806ea3.img.jpg_256x160_659f7c33.jpg',
            title: '少林寺',
            desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
            money: '5'
          },
          {
            id: '0005',
            imgUrl: 'http://img1.qunarzz.com/sight/p0/1709/e9/e9b7ae23f567806ea3.img.jpg_256x160_659f7c33.jpg',
            title: '少林寺',
            desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
            money: '5'
          }, {
            id: '0006',
            imgUrl: 'http://img1.qunarzz.com/sight/p0/1709/e9/e9b7ae23f567806ea3.img.jpg_256x160_659f7c33.jpg',
            title: '少林寺',
            desc: '登顶中岳嵩山，一览天下胜景，领略禅宗教法',
            money: '5'
          }, {
            id: '0007',
            imgUrl: 'http://img1.qunarzz.com/sight/p0/1709/e9/e9b7ae23f567806ea3.img.jpg_256x160_659f7c33.jpg',
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

  .item
    display: flex;
    height: 1.9rem;
    overflow: hidden;

    .item-img
      width: 1.7rem;
      height: 1.7rem;
      padding: 0.1rem;

    .item-info
      flex: 1;
      padding: .1rem
      min-width: 0;

    .item-title
      line-height: .54rem
      font-size: .32rem
      overflow: hidden
      white-space: nowrap;
      text-overflow: ellipsis

    .item-desc
      line-height: .4rem;
      color: #ccc
      overflow: hidden
      white-space: nowrap;
      text-overflow: ellipsis;
      position: relative

    .item-end
      margin-top: .16rem
      display: inline-block
      width: 100%;

    .item-money
      color: #ff9300;
      line-height: .5rem
      font-size: .48rem
      font-weight: 550
      vertical-align: middle;

    .item-button
      position: absolute
      color: #ffffff
      background: #ff9300;
      border-radius: 0.16rem;
      padding: 0.1rem;
      line-height: .44rem;
      vertical-align: middle;
      right: .5rem;

</style>
