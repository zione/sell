<template>
  <div>
    <detail-banner></detail-banner>
    <detail-header></detail-header>
    <detail-list :list="list"></detail-list>
  </div>
</template>

<script>
import DetailBanner from './component/Banner'
import DetailHeader from './component/header'
import DetailList from './component/List'
export default {
  name: 'Detail',
  components: {
    DetailBanner,
    DetailHeader,
    DetailList
  },
  data () {
    return {
      list: [{
        title: '成人票',
        children: [{
          title: '承认五观联票',
          children: [
            {
              title: '城隍庙'
            }
          ]
        },
        {
          title: '承认六观联票'
        }]
      },
      {
        title: '学生票',
        children: [{
          title: '承认三观联票'
        },
        {
          title: '承认五观联票'
        },
        {
          title: '承认六观联票'
        }]
      },
      {
        title: '儿童票',
        children: [{
          title: '承认三观联票'
        },
        {
          title: '承认五观联票'
        },
        {
          title: '承认六观联票'
        }]
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .content
    height: 50rem
</style>
