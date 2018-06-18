<template>
  <div>
    <div class="banner" @click="handleBannerClick">
      <img class="banner-img" src="https://img1.qunarzz.com/p/tts7/201408/09/e8e2cce49768d8aec8d65eac.jpg_r_640x420x90_0e8a9b73.jpg">
      <div class="banner-info">
        <div class="banner-tittle">大连圣亚海洋（AAAA景区）</div>
        <div class="banner-number">
          <span class="iconfont banner-icon">&#xe626;</span>
          32
        </div>
      </div>
    </div>
    <common-gallary
      :imgs="imgs"
      v-show="showGallary"
      @closeGallary = "handleGallaryClose"
    >
    </common-gallary>
  </div>
</template>

<script>
import CommonGallary from 'common/gallary/Gallary'
export default {
  name: 'DetailBanner',
  components: {
    CommonGallary
  },
  data () {
    return {
      showGallary: false,
      imgs: [
        'https://img1.qunarzz.com/p/tts7/201408/09/e8e2cce49768d8aec8d65eac.jpg_r_640x420x90_0e8a9b73.jpg',
        'https://img1.qunarzz.com/p/tts7/201408/09/e8e2cce49768d8aec8d65eac.jpg_r_640x420x90_0e8a9b73.jpg'
      ]
    }
  },
  methods: {
    handleBannerClick () {
      this.showGallary = true
    },
    handleGallaryClose () {
      this.showGallary = false
    }
  }
}
</script>

<style lang="stylus" scoped>
  .banner
    position: relative
    overflow: hidden
    height: 0
    padding-bottom: 55%
    .banner-img
      width: 100%
    .banner-info
      align-items: center
      display: flex
      position: absolute
      left: 0
      right: 0
      bottom: 0
      line-height: .6rem
      color: #ffffff
      background-image: linear-gradient(top,rgba(0,0,0,0),rgba(0,0,0,.8))
      .banner-tittle
        flex-grow: 1
        font-size: .32rem
        padding: 0 .2rem
      .banner-number
        padding: 0 .2rem
        line-height: .32rem
        height: .32rem
        border-radius: .2rem
        font-size: .24rem
        background: rgba(0,0,0,.8)
        .banner-icon
          font-size: .24rem
</style>
