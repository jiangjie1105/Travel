<template>
    <div class="header">
        <div class="header-left">
            <div class="iconfont back-icon">&#xe624;</div>
        </div>
        <div class="header-input">
            <span class="iconfont">&#xe632;</span>
            输入城市/景点/游玩主题
        </div>
        <div class="header-rignt">城市
            <div class="iconfont down-icon">&#xe62d;</div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>//scoped表示只对当前页面样式有影响
  @import '~styles/varibles.styl'
  .header
    display :flex
    height: .86rem
    background :$bgColor
    color :#fff
    .header-left
      display: flex
      justify-content :center
      align-items :center
      width: .64rem
      float: left
      .back-icon
        font-size: .20rem
    .header-input
      flex: 1
      height :.64rem
      line-height :.64rem
      color :black
      background-color  : #fff
      margin-top: .12rem
      margin-left: .2rem
      padding-left: .2rem
      border-radius: .1rem
    .header-rignt
      display: flex
      justify-content: center;
      align-items: center;
      width :1.24rem
      float: right
      text-align: center
      .down-icon
        font-size: .2.3rem
</style>
