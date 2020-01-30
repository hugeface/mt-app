<template>
  <div class="m-menu">
    <el class="nav">
      <dt>全部分类</dt>
      <dd
        v-for="(item, index) in menu"
        :key="index"
      >
        <i :class="item.type" /> {{ item.name }}<span class="arrow" />
      </dd>
    </el>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data () {
    return {
      menu: [{
        type: 'food',
        name: '美食',
        child: [{
          title: '美食',
          child: ['代金券', '甜点饮品', '火锅', '自助餐', '小吃快餐']
        }]
      }, {
        type: 'takeout',
        name: '外卖',
        child: [{
          title: '外卖',
          child: ['美团外卖']
        }]
      }, {
        type: 'hotel',
        name: '酒店',
        child: [{
          title: '酒店星级',
          child: ['经济型', '舒适/三星', '高档/四星', '豪华/五星']
        }]
      }]
    }
  }
})
</script>
