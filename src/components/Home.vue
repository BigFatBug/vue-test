<template>
  <div style="font-family: fengbi">
  <el-container>
    <home-header></home-header>
    <div class="header-line"></div>
    <el-main>
      <el-row :gutter="20">
        <el-col :span="5">
          <home-person></home-person>
        </el-col>
        <el-col :span="14">
          <home-video></home-video>
        </el-col>
        <el-col :span="5"><home-video-list></home-video-list></el-col>
      </el-row></el-main>
    <el-footer></el-footer>
  </el-container>
  </div>
</template>

<style>
  .el-footer {
    background-color: #B3C0D1;
    color: #333;
    text-align: center;
    line-height: 60px;
  }
  .header-line{
    height: 5px;
    background-color: #00d1b2;
  }
  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }

</style>
<script>
  import HomeHeader from './HomeHeader.vue'
  import HomePerson from './HomePerson.vue'
  import HomeVideo from './HomeVideo.vue'
  import HomeVideoList from './HomeVideoList.vue'
  import ElMain from "../../node_modules/element-ui/packages/main/src/main.vue";
  import ElFooter from "../../node_modules/element-ui/packages/footer/src/main.vue";

  export default {
    components: {
      ElFooter,
      ElMain,
      HomeHeader,
      HomePerson,
      HomeVideo,
      HomeVideoList
    },
    methods: {
      header(path){

      }
    }
  }
</script>
