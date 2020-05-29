<template>
  <div>
    <div class="title">热销推荐</div>
      <ul>
        <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
            <img class="item-img" :src="item.imgUrl" />
            <div class="item-info">
              <p class="item-title">{{item.title}}</p>
              <p class="item-desc">{{item.desc}}</p>
              <button class="item-button">查看详情</button>
            </div>
        </li>
      </ul>
  </div>
</template>

<script>
export default {
  name: 'Homerecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'https://imgs.qunarzz.com/sight/p0/1504/59/594e60a1366e1741.water.jpg_200x200_b1e2d39d.jpg',
        title: '加加加及i氨甲基',
        desc: 'hhhhhhhhhhahahahahhahahhhah'
      }, {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/sight/p0/1504/59/594e60a1366e1741.water.jpg_200x200_b1e2d39d.jpg',
        title: '加加加及i氨甲基',
        desc: 'hhhhhhhhhhahahahahhahahhhah'
      }, {
        id: '0003',
        imgUrl: 'https://imgs.qunarzz.com/sight/p0/1504/59/594e60a1366e1741.water.jpg_200x200_b1e2d39d.jpg',
        title: '加加加及i氨甲基',
        desc: 'hhhhhhhhhhahahahahhahahhhah'
      }, {
        id: '0004',
        imgUrl: 'https://imgs.qunarzz.com/sight/p0/1504/59/594e60a1366e1741.water.jpg_200x200_b1e2d39d.jpg',
        title: '加加加及i氨甲基',
        desc: 'hhhhhhhhhhahahahahhahahhhah'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    margin-top: .2rem
    line-height : .8rem
    background: #eee
  .item
    overflow: hidden
    display: flex
    height: 1.9rem
    .item-img
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    .item-info
      flex: 1
      padding : .1rem
      min-width: 0
      .item-title
        line-height : .54rem
        font-size: .32rem
        ellipsis()
      .item-desc
        line-height :.4rem
        color :#ccc
        ellipsis()
      .item-button
        line-height: .44rem
        background : #ff9300
        margin-top : .2rem
        padding : 0 .2rem
        border-radius: .06rem
        color: #fff
</style>
