<template>
  <div class="page">
    <div>calculation</div>
    <div
      class="show-box-bar"
      @click="changeBoxStatus"
      v-show="!showInputBox"
    >
      show
    </div>
    <div class="input-box" v-show="showInputBox">
      <div class="hide-box-bar" @click="changeBoxStatus">hide</div>
      <div class="box">
        <input-box></input-box>
      </div>
    </div>
  </div>
</template>

<script>
import inputBox from './components/inputBox'

export default {
  data () {
    return {
      showInputBox: true
    }
  },

  components: {
    inputBox
  },

  methods: {
    changeBoxStatus () {
      this.showInputBox = !this.showInputBox
    }
  },

  created () {
    // let app = getApp()
  }
}
</script>

<style scoped>
  .show-box-bar {
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
    display: block;
    margin: auto auto;
    width: fit-content;
    padding: 15rpx;
    background-color: #ee22cc;
  }
  .input-box {
    position: absolute;
    width: 100%;
    height: 600rpx;
    bottom: 0;
    z-index: 200;
    background-color: #01de33;
  }
  .input-box > .hide-box-bar {
    display: block;
    width: fit-content;
    margin: auto auto;
    padding: 15rpx;
    background-color: #e42929;
  }
  .input-box > .box {
    background-color: #2323ff;
  }
</style>
