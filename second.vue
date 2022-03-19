<template>
<el-container>
  <el-header class="biaoti" style="height:60px;">
    <span class="biaoti1">网 课 百 问 解 答</span>
     <span class="touxiang">
      <el-button @click="tuichu">返回类别</el-button>
    </span>
    
   
  </el-header>


  <el-container class="contain">
      <!-- <div class="video-wrap" style="width:80%;float:left;oveflow:hidden;">
         <iframe :src="../assets/zhineng.mp4" frameborder='0'
          allow='autoplay;encrypted-media' allowfullscreen style='width:100%;height:500px;'>
         </iframe>

       </div>  -->
  </el-container>

</el-container>
</template>



<script>
//  import asidess from '@/views/asidess'


  export default {
    data() {
      return {
        activeIndex: '1',
        activeName: '',
      };
    },
    components:{
      // asidess,
      // card,
      // xinxi,
      // table
    },
    methods: {
      // handleSelect(key, keyPath) {
      //   console.log(key, keyPath);
      // },
      tuichu(){
        this.$router.push('/');  
      }
    }
  }

 

 
</script>
<style scoped>
 /* lang="scss" scoped */
.contain{
  width: 700px;
  margin: auto;

 
}

   ::v-deep .el-collapse-item__header{
        line-height: initial;
        font-size: 16px;
          font-family:'微软雅黑', Times, serif;
          height: 70px;

    }
    ::v-deep .el-collapse-item__content{
        font-size: 15px;
          font-family:'微软雅黑', Times, serif;

    }

.biaoti{
  background-color:#353536;
  position: fixed;
  width: 100%;
  height: 40px;
  
}

.biaoti1{
  font-size: 25px;
  margin: 0px 0px 0px 20px;
  line-height: 60px;
  text-align: center;
  color: #ffcf4bf1;
  font-family:'微软雅黑', Times, serif;
}
.el-menu-item is-active{
  height: 30px;

}


.el-aside{
  min-height: 650px;
  background-color:#353536;
  
  
}
.touxiang{
  margin: 15px 50px 0px 0px;
  float: right;
}

</style>