<template>
  <div>
    <div class="welcome">欢迎使用gpaCalculator</div>
    <div class="welcome">请首先设置参数</div>
    <form>
      <label>
        <radio-group>
          <span class="label">满绩：</span>
          <radio class="radio" value="4">4.0</radio>
          <radio class="radio" value="5">5.0</radio>
        </radio-group>
      </label>
    </form>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  },

  methods: {
  },

  created () {
    // let app = getApp()
  }
}
</script>

<style scoped>
  .welcome {
    text-align: center;
  }
  .label {
    display: inline;
    margin-left: 30rpx;
  }
  .radio {
    margin: 15rpx;
  }
</style>
