<template>
    <div>
      <form>
        <label>
          <radio-group>
            <span class="label">算法</span>
            <radio class="radio" value="4">标准4.0</radio>
            <radio class="radio" value="5">5.0</radio>
          </radio-group>
        </label>
      </form>
    </div>
</template>

<script>
export default {
  created () {
    // let app = getApp()
  }
}
</script>

<style scoped>
  .label {
    display: inline;
    margin-left: 30rpx;
  }
  .radio {
    margin: 15rpx;
  }
</style>
