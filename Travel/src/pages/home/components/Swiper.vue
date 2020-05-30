<template>
    <swiper :options="swiperOptions" v-if= "list.length">
      <swiper-slide v-for="item of list" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl">
      </swiper-slide>
        <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
</template>

<script>
export default {
  name: 'HomeSwiper',
  props: {
    list: Array
  },
  data () {
    return {
      swiperOptions: {
        pagination: '.swiper-pagination',
        loop: true
      },
      // computed: {
      //   showSwiper () {
      //     return this.list.length
      //   }
      // },此功能是代替在模板中写语法的功能
      swiperList: [{
        id: '0001',
        imgUrl: 'https://imgs.qunarzz.com/sight/p0/1907/cd/cdb4c750676d6d02a3.img.jpg_710x360_c4abf30c.jpg'
      }, {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/sight/p0/1707/20/20795ed07a91c875a3.water.jpg_710x360_b891382e.jpg'
      }]
    }
  }
}
</script>

<style lang = "stylus" scoped>
  .swiper-img
    width: 100%
</style>
