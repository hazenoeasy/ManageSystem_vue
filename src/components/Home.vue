<template>
  <div>
    <el-button type = "info" @click="clearToken"> 退出 </el-button>
  </div>
</template>

<script>
export default {
  methods: {
    clearToken () {
      window.sessionStorage.clear()
      this.$router.push('/login')
    }
  }
}
</script>

<style lang= "less" scoped>
</style>
