<template>
  <h1>组件</h1>

  <h2>hello world</h2>
  <HelloWorld/>

  <h2>向子组件传递数据</h2>
  <props/>

</template>
<script>

import HelloWorld from "@/views/components/helloworld/index"
import Props from "@/views/components/props/parent"

export default {
  name: "components",
  components: {
    HelloWorld,
    Props
  }
}
</script>

<style scoped>

</style>
