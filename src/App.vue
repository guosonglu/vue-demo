<template>
  <div>
    <el-tabs v-model="activeName">
      <el-tab-pane label="组件示例" name="first">
        <component-demo/>
      </el-tab-pane>
      <el-tab-pane label="路由示例" name="second">

      </el-tab-pane>
      <el-tab-pane label="Vuex示例" name="third">

      </el-tab-pane>
    </el-tabs>
  </div>
</template>

<script>
import ComponentDemo from "@/views/components/index"

export default {
  name: 'App',
  components: {
    ComponentDemo
  },
  data() {
    return {
      activeName: 'first',
    }
  },

}
</script>

<style>

</style>
