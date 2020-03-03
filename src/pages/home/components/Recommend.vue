<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul>
      <li class="item border-bottom">
        <img class="item-img"
             src="http://img1.qunarzz.com/sight/p0/1709/e9/e9b7ae23f567806ea3.img.jpg_256x160_659f7c33.jpg">
        <div class="item-info">
          <p class="item-title">少林寺 </p>
          <p class="item-desc">登顶中岳嵩山，一览天下胜景，领略禅宗教法</p>
          <p class="item-money"></p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    name: 'HomeRecommend'
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

    .item-title
      line-height: .54rem
      font-size: .32rem

    .item-desc
      line-height: .4rem;
      color: #ccc
      overflow: hidden
      white-space: nowrap;
      text-overflow: ellipsis
      width: 93%

</style>
