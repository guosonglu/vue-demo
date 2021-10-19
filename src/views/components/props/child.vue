<template>
  <div>传入静态字符串：{{ title1 }}</div>
  <div>传入变量字符串：{{ title2 }}</div>

  <div>传入静态数字，父组件仍然需要`v-bind`或`:`来告诉Vue这是一个 JavaScript 表达式而不是一个字符串:{{ likes1 }}</div>
  <div>传入变量数字：{{ likes2 }}</div>

  <div>布尔值不传值默认为：{{ isPublished1 }}</div>
  <div>传入静态布尔值，父组件仍然需要`v-bind`或`:`来告诉Vue这是一个 JavaScript 表达式而不是一个字符串:{{ isPublished2 }}</div>
  <div>传入变量布尔值：{{ isPublished3 }}</div>

  <div>传入静态数组，父组件仍然需要`v-bind`或`:`来告诉Vue这是一个 JavaScript 表达式而不是一个字符串:{{ commentIds1 }}</div>
  <div>传入变量数组：{{ commentIds2 }}</div>

  <div>传入静态对象，父组件仍然需要`v-bind`或`:`来告诉Vue这是一个 JavaScript 表达式而不是一个字符串:{{ author1 }}</div>
  <div>传入变量对象：{{ author2 }}</div>
  <div>传入对象的所有property:{{name}} {{company}}</div>
</template>

<script>
export default {
  name: "child",
  props: {
    title1: String,
    title2: String,
    likes1: Number,
    likes2: Number,
    isPublished1: Boolean,
    isPublished2: Boolean,
    isPublished3: Boolean,
    commentIds1: Array,
    commentIds2: Array,
    author1: Object,
    author2: Object,
    name: String,
    company: String
  }
}
</script>

<style scoped>

</style>
