<template>
  <child
      title1="静态字符串"
      :title2="title"

      :likes1="10"
      :likes2="like"

      is-published1
      :is-published2="true"
      :is-published3="isPublished"

      :comment-ids1="[234, 266, 273]"
      :comment-ids2="commentIds"

      :author1="{name: 'Veronica',company: 'Veridian Dynamics'}"
      :author2="author"
      :="author"


  />
</template>

<script>
import Child from "./child"

export default {
  name: "parent",
  components: {
    Child
  },
  data() {
    return {
      title: "变量字符串",
      like: 20,
      isPublished: false,
      commentIds: [10, 20, 30],
      author: {
        name: "张三",
        company: "alibaba"
      }
    }
  }
}
</script>

<style scoped>

</style>
