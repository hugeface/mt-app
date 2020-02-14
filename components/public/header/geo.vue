<template>
  <div class="m-geo">
    <i class="el-icon-location" /> {{ $store.state.geo.position.city }}
    <nuxt-link
      class="changeCity"
      to="changeCity"
    >
      切换城市
    </nuxt-link>
    [金华 永康 义乌]
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({

})
</script>

<style lang="sass" scoped>

</style>
