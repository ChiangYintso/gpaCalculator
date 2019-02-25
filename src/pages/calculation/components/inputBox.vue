<template>
  <div>
    <div class="num-btn" v-for="(item,index) of arr" :key="index">
      <button>{{item}}</button>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      arr: [1, 2, 3, 4, 5, 6, 7, 8, 9]
    }
  }
}
</script>

<style scoped>
  .num-btn {
    width: 33.33%;
    display: inline-block;
    overflow: hidden;
  }
</style>
