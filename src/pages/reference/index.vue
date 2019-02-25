<template>
    <div>
      <div class="headline">计算前请先在“设置”中确认参数。</div>
      <div class="equation">平均学分绩点=∑(课程学分×成绩绩点)/∑课程学分</div>
    </div>
</template>

<script>
export default {
  created () {
    // let app = getApp()
    console.log(this.$store.state.test)
  }
}
</script>

<style scoped>
  .headline {
    text-align: center;
    font-size: 36rpx;
    margin: 20rpx;
  }
  .equation {
    font-size:28rpx;
    margin: 20rpx;
    color: #a32020;
  }
</style>
