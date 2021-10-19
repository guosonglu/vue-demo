<template>
  <div>
    <button @click="count++">
      You clicked me {{ count }} times.
    </button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      count: 0
    }
  }
}
</script>

<style scoped>

</style>
