<template>
  <div>
    <div>calculation</div>
    <div class="input-box">
      <input-box></input-box>
    </div>
  </div>
</template>

<script>
import inputBox from './components/inputBox'
export default {
  data () {
    return {
    }
  },

  components: {
    inputBox
  },

  methods: {
  },

  created () {
    // let app = getApp()
  }
}
</script>

<style scoped>
  .input-box {
    position: absolute;
    width: 100%;
    height: 600rpx;
    bottom: 0;
    z-index: 200;
    background-color: #01de33;
  }
</style>
