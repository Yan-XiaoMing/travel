<template>
  <div>
    <detail-banner/>
    <detail-header/>
    <div class="content"></div>
  </div>
</template>

<script>
  import DetailBanner from './components/Banner';
  import DetailHeader from './components/Header';

  export default {
    name: 'Detail',
    components: {DetailHeader, DetailBanner}
  };
</script>

<style scoped lang="stylus">
  .content
    height: 50rem
</style>
