<template>
  <div>
    <home-header></home-header>
    <home-swiper :list="swiperList"></home-swiper>
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
  },
  data () {
    return {
      swiperList: [{
        id: '0001',
        imgUrl: 'https://imgs.qunarzz.com/p/tts3/1703/e3/3d71ff582f05e802.jpg_r_390x260x90_7c8b1419.jpg'
      },
      {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/p/tts0/1511/60/4b101da07eb663f7.jpg_r_390x260x90_ce705dbf.jpg'
      }]
    }
  }
}
</script>

<style scoped>

</style>
