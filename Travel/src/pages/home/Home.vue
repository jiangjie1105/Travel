<template>
    <div>
    <!--这里遇到一个坑，必须在template模板中再加一个div标签才可以-->
    <home-header></home-header>
    <home-swiper></home-swiper>
    </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwiper
  }
}
</script>

<style>

</style>
