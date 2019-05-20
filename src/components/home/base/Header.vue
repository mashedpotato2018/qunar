<template>
    <div class="header">
        <i class="iconfont icon-fanhui header-back"></i>
      <div class="header-input">
        <i class="iconfont icon-sousuo"></i>
        <input type="text" placeholder="输入城市/景点/游玩主题">
      </div>
      <div class="header-right">
        <span>成都</span><i class="iconfont icon-jiantou"></i>
      </div>
    </div>
</template>

<script>
    export default {
      name:'HomeHeader',
        data() {
            return {}
        }
    }
</script>

<style lang="stylus" scoped>
  .header
    display flex
    align-items center
    height .88rem
    background-color #00bcd4
    line-height .88rem
    color #fff
    .header-back
      width .88rem
      text-align center
    .header-input
      flex 1
      padding-left .1rem
      background-color #fff
      line-height .56rem
      border-radius .1rem
      .icon-sousuo
        color #ccc
        vertical-align middle
      input
        font-size .26rem
      input::placeholder
        color #eee

    .header-right
      padding 0 .2rem
      .icon-jiantou
        font-size .24rem
        vertical-align 4%
</style>
