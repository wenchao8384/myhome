<template>
  <div class='navBarWrap'>
    <el-carousel indicator-position="none" autoplay="false" interval='5000'>
      <el-carousel-item v-for="item in 4" :key="item"> 
        <div class='navBar'>
           <div>
             <img src="../assets/banner2.png" alt="">
            </div>
            <div class='navText'>
              <div>I'm passionate about food, the tradition of it, cooking it, sharing it</div>
              <p>by <b> Sean Hamilton, Patricia Jenkins, James Bryant</b> 3 years ago</p>
              <i class='el-icon-time'>1 MIN READ</i>
            </div>
        </div>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
export default {
}
  </script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.el-carousel__item h3 {
    color: #475669;
    font-size: 18px;
    opacity: 0.75;
    line-height: 400px;
    margin: 0;
  }
  .navBarWrap>div{
    margin-top:50px;
    width:95%;
    margin-left:80px;
  }
  .navBar{
    display: flex;
  }
  .navBar>div{
    flex: 1;
  }
  .navText{
    text-align: letf;
  }
  .navText>div{
    width: 550px;
    margin-top: 120px;
    font-size: 50px;
    font-weight: 600;
  }
  .navText>i{
    color: darkgray;
    font-size: 14px;
  }
</style>
<style>
.navBarWrap>div .el-carousel__container{
    height:550px!important;
  }
</style>
