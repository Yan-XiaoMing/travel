<template>
  <div class="search">
    <input type="text" placeholder="输入城市名或拼音" class="search-input">
  </div>
</template>

<script>
  export default {
    name: 'CitySearch.vue'
  };
</script>

<style scoped lang="stylus">
  .search
    height: .72rem
    background: #00bcd4
    padding: 0 .1rem

    .search-input
      box-sizing : border-box
      height: .62rem
      width: 100%
      padding :0 .1rem
      line-height: .62rem
      text-align: center
      border-radius: .06rem
      color :#666

</style>
