<template>
  <div>
    <div class="title">周末去哪儿</div>
      <ul>
        <li class="item border-bottom" v-for="item of list" :key="item.id">
            <div class="item-img-wrapper">
              <img class="item-img" :src="item.imgUrl" />
            </div>
            <div class="item-info">
              <p class="item-title">{{item.title}}</p>
              <p class="item-desc">{{item.desc}}</p>
            </div>
        </li>
      </ul>
  </div>
</template>

<script>
export default {
  name: 'HomereWeekend',
  props: {
    list: Array
  }
  // data () {
  //   return {
  //     recommendList: [{
  //       id: '0001',
  //       imgUrl: 'https://imgs.qunarzz.com/sight/source/1509/10/d4f702d538b8d4.jpg_r_640x214_8a88df87.jpg',
  //       title: '加加加及i氨甲基',
  //       desc: 'hhhhhhhhhhahahahahhahahhhah'
  //     }, {
  //       id: '0002',
  //       imgUrl: 'https://imgs.qunarzz.com/sight/p0/1504/59/594e60a1366e1741.water.jpg_200x200_b1e2d39d.jpg',
  //       title: '加加加及i氨甲基',
  //       desc: 'hhhhhhhhhhahahahahhahahhhah'
  //     }, {
  //       id: '0003',
  //       imgUrl: 'https://imgs.qunarzz.com/sight/p0/1504/59/594e60a1366e1741.water.jpg_200x200_b1e2d39d.jpg',
  //       title: '加加加及i氨甲基',
  //       desc: 'hhhhhhhhhhahahahahhahahhhah'
  //     }, {
  //       id: '0004',
  //       imgUrl: 'https://imgs.qunarzz.com/sight/p0/1504/59/594e60a1366e1741.water.jpg_200x200_b1e2d39d.jpg',
  //       title: '加加加及i氨甲基',
  //       desc: 'hhhhhhhhhhahahahahhahahhhah'
  //     }]
  //   }
  // }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    line-height : .8rem
    background: #eee
    text-indent: .2rem
  .item-img-wrapper
    overflow: hidden
    height: 0
    padding-bottom: 37.09%
    .item-img
      width: 100%
  .item-info
    padding : .1rem
  .item-title
    line-height : .54rem
    font-size: .32rem
    ellipsis()
  .item-desc
    line-height :.4rem
    color :#ccc
    ellipsis()
</style>
