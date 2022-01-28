<template>
  <el-menu :default-active="activeIndex2"
    class="el-menu-demo"
    mode="horizontal"
    @select="handleSelect"
    background-color="#184D47"
    text-color="#fff"
    active-text-color="#ffd04b">
    <el-row >
      <el-col :span="5"><el-menu-item class="myHome" index="1">JAMES ANGELO SUAREZ ERGINA</el-menu-item></el-col>
      <el-col :span="2" offset="13">
        <el-submenu index="2">
          <template slot="title">About Me</template>
          <el-menu-item index="2-1">Personal Info</el-menu-item>
          <el-menu-item index="2-2">Organizational Affiliations</el-menu-item>
          <el-menu-item index="2-3">Educational Background</el-menu-item>
        </el-submenu>
      </el-col>
      <el-col :span="2"><el-menu-item index="3">Experiences</el-menu-item></el-col>
      <el-col :span="2"><el-menu-item index="4"><a>Contact Me</a></el-menu-item></el-col>
    </el-row>
  </el-menu>
</template>

<script>
  export default {
    data() {
      return {
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style scoped>
.myHome{
  text-align: left;
}

el-menu-item{
  text-align: center;
}


</style>
