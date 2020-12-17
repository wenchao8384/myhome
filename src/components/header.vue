<template>
  <div>
     <div class='title'>布朗熊</div>
     <el-menu text-color="#333333" active-text-color='#5d5353' :default-active="activeIndex" class="el-menu-demo headerNav" mode="horizontal" @select="handleSelect">
      <el-menu-item index="1">首页</el-menu-item>
      <el-submenu index="2">
        <template slot="title">诗和远方</template>
        <el-menu-item index="2-1">美食</el-menu-item>
        <el-menu-item index="2-2">旅行</el-menu-item>
      </el-submenu>
      <el-menu-item index="3">又是板砖的一天</el-menu-item>
      <el-menu-item index="4">甜甜的恋爱</el-menu-item>
     <el-submenu index="5">
        <template slot="title">更多</template>
        <el-menu-item index="5-1">。。</el-menu-item>
        <el-menu-item index="5-2">。。</el-menu-item>
      </el-submenu>
      <div class='signawrap'>
         <el-button size="small" circle>sign in</el-button>
         <el-button type="primary" size="small" circle>sign up</el-button>
         <i class="el-icon-search search"></i>
      </div>   
    </el-menu>
    <div class="line"></div>
    <div class='sign'>THOUGHTS, STORIES AND IDEAS</div>
  </div>
</template>

<script>
export default {
    data() {
      return {
        activeIndex: '1',
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.title{
  float:left;
  margin-left:150px;
  font-size:30px;
   margin-top:15px;
}
.headerNav{
  float:right;
  margin-right:150px;
  font-size:26px!important;
  margin-bottom: 20px;
}
.signawrap{
  float:right;
  margin-top:10px;
}
.search{
  margin-left:15px;
  line-height:30px;
}
.sign{
  transform:rotate(270deg);
  position:fixed;
  top: 306px;
  left: -79px;
}
</style>
