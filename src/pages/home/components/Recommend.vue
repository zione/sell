<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl">
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
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0000',
        imgUrl: 'https://ss0.bdstatic.com/-0U0bnSm1A5BphGlnYG/tam-ogel/38cd7a459e6d92cc4d87629645ac81fb_78_59.jpg',
        title: '大连圣亚海浪漫的海洋浪漫的海洋洋世界',
        desc: '浪漫大连首站，浪漫的海洋浪漫的海洋浪漫的海洋主题乐园'
      }, {
        id: '0001',
        imgUrl: 'https://ss0.bdstatic.com/-0U0bnSm1A5BphGlnYG/tam-ogel/38cd7a459e6d92cc4d87629645ac81fb_78_59.jpg',
        title: '大连圣亚海浪漫的海洋浪漫的海洋洋世界',
        desc: '浪漫大连首站，浪漫的海洋浪漫的海洋浪漫的海洋主题乐园'
      }, {
        id: '0002',
        imgUrl: 'https://ss0.bdstatic.com/-0U0bnSm1A5BphGlnYG/tam-ogel/38cd7a459e6d92cc4d87629645ac81fb_78_59.jpg',
        title: '大连圣亚海浪漫的海洋浪漫的海洋洋世界',
        desc: '浪漫大连首站，浪漫的海洋浪漫的海洋浪漫的海洋主题乐园'
      }, {
        id: '0003',
        imgUrl: 'https://ss0.bdstatic.com/-0U0bnSm1A5BphGlnYG/tam-ogel/38cd7a459e6d92cc4d87629645ac81fb_78_59.jpg',
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
  .item
    display: flex
    height: 1.9rem
    overflow: hidden
    .item-img
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    .item-info
      min-width: 0
      flex-grow: 1
      padding: .1rem
      .item-title
        line-height: .54rem
        font-size: .32rem
        ellipsis()
      .item-desc
        line-height: .54rem
        color: #ccc
        ellipsis()
      .item-button
        margin-top: .2rem
        background: #ff9300
        padding: 0 .2rem
        border-radius: .06rem
        color: #ccc
</style>
