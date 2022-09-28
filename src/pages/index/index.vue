<template>
  <div>
    <span class="msg">Hello,world!</span>

    <van-button type="primary" @click="jump">按钮</van-button>
  </div>
</template>

<script>
  import { post } from '@/utils/request.js'

  export default {
    methods: {
      jump() {
        // this.$router.push('/pages/index/main')
        post('https://www.baidu.com').then(response => {
          console.log('getresponse!')
        })
      }
    }
  }
</script>

<style lang="scss" scoped>
.msg{
  color: lightblue;
}
</style>
