<template>
    <div>
      this is index.vue
    </div>
</template>
<script>
export default{
  data () {
    return {
      msg: 'hello vue'
    }
  },
  components: {},
  created () {
    this.$api.get('topics', null, r => {
      console.log(r)
    })
  }
}
</script>
<style>

</style>
