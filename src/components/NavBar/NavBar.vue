<template>
  <div class="nav-bar">
    <router-link tag="div" class="tab-item" :to="{name: 'Recommend'}" replace>
      <span class="tab-link">推荐</span>
    </router-link>
    <router-link tag="div" class="tab-item" :to="{name: 'SingerList'}" replace>
      <span class="tab-link">歌手</span>
    </router-link>
    <router-link tag="div" class="tab-item" :to="{name: 'RankList'}" replace>
      <span class="tab-link">排行
      </span>
    </router-link>
    <router-link tag="div" class="tab-item" :to="{name: 'Search'}" replace>
      <span class="tab-link">搜索</span>
    </router-link>
  </div>
</template>

<script type="text/ecmascript-6">
  export default {}
</script>

<style lang="stylus" type="text/stylus">
  @import "../../assets/stylus/variable2.styl";

  .nav-bar
    display flex
    height 44px
    line-height 44px
    font-size $font-size-medium
    background-color $color-bg
    .tab-item
      flex 1
      text-align center
      .tab-link
        padding-bottom 5px
        color $color-font-d
      &.router-link-active
        .tab-link
          color $color-theme
          border-bottom 2px solid $color-theme
</style>
