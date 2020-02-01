<template>
  <div class="page-index">
    <el-row>
      <el-col :span="5">
        <emenu />
      </el-col>
      <el-col :span="19">
        <elife />
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="24">
        <artistic />
      </el-col>
    </el-row>
  </div>
</template>

<script>
import Vue from 'vue'
import Emenu from '@/components/index/menu.vue'
import Elife from '@/components/index/life.vue'
import Artistic from '@/components/index/artistic.vue'
export default Vue.extend({
  components: { Emenu, Elife, Artistic }
})
</script>

<style lang="scss">
  @import "@/assets/css/index/index.scss";
</style>
