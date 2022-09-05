<template> 
<view>
  <button class="btn" @tap="toTest">跳转到测试页面</button>
</view>
</template>

<script setup lang="ts">
  import Taro from '@tarojs/taro'
  const toTest = () => {
    Taro.navigateTo({
      url: '/pages/testpage/index'
    })
  }
</script>
<style lang="less">
  .btn{
    width: 100%;
    height: 100rpx;
    background-color: #eee;
  }
</style>