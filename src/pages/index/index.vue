<template>
  <div>
    <span class="msg">Hello,world!</span>
    <van-button type="primary" @click="jump">按钮</van-button>
  </div>
</template>

<script>
export default {
  methods: {
    jump () {
      this.$router.push('/pages/index/main')
    }
  }
}
</script>

<style lang="scss" scoped>
.msg{
  color: lightblue;
}
</style>
