<template>
  <div>
    <div class="recommend-title">周末去哪儿</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl">
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
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [{
        id: '0000',
        imgUrl: 'https://imgs.qunarzz.com/p/p17/1801/ab/73306c5650ba9802.jpg',
        title: '大连圣亚海浪漫的海洋浪漫的海洋洋世界',
        desc: '浪漫大连首站，浪漫的海洋浪漫的海洋浪漫的海洋主题乐园'
      }, {
        id: '0001',
        imgUrl: 'https://imgs.qunarzz.com/p/p17/1801/ab/73306c5650ba9802.jpg',
        title: '大连圣亚海浪漫的海洋浪漫的海洋洋世界',
        desc: '浪漫大连首站，浪漫的海洋浪漫的海洋浪漫的海洋主题乐园'
      }, {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/p/p17/1801/ab/73306c5650ba9802.jpg',
        title: '大连圣亚海浪漫的海洋浪漫的海洋洋世界',
        desc: '浪漫大连首站，浪漫的海洋浪漫的海洋浪漫的海洋主题乐园'
      }, {
        id: '0003',
        imgUrl: 'https://imgs.qunarzz.com/p/p17/1801/ab/73306c5650ba9802.jpg',
        title: '大连圣亚海浪漫的海洋浪漫的海洋洋世界',
        desc: '浪漫大连首站，浪漫的海洋浪漫的海洋浪漫的海洋主题乐园'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import "~styles/mixins.styl"
  .recommend-title
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
  .item-img-wrapper
    overflow: hidden
    height: 0
    padding-bottom: 33.3%
    .item-img
      width: 100%
  .item-info
    padding: .1rem
    .item-title
      line-height: .54rem
      font-size: .32rem
      ellipsis()
    .item-desc
      line-height: .54rem
      color: #ccc
      ellipsis()
</style>
