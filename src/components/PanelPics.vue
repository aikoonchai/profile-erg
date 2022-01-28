<template>
    <el-carousel indicator-position="inside" height="100px" arrow="hover">
        <el-carousel-item v-for="item in 4" :key="item">
        </el-carousel-item>
    </el-carousel>
</template>

<script>
  export default {
  }
</script>

<style scoped>
  .el-carousel__item:nth-child(2n) {
    background-color: #00917C;
  }
  .el-carousel__item:nth-child(2n+1) {
    background-color: #035956;
  }
</style>
