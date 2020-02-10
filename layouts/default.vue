<template>
  <el-container class="layout-default">
    <el-header>
      <my-header />
    </el-header>
    <el-main>
      <div>
        <nuxt />
      </div>
    </el-main>
    <el-footer>
      <my-footer />
    </el-footer>
  </el-container>
</template>

<script>
import Vue from 'vue'
import MyHeader from '@/components/public/header'
import MyFooter from '@/components/public/footer'
export default Vue.extend({
  components: { MyHeader, MyFooter }
})
</script>
