<template>
<el-container>
  <el-header class="biaoti" style="height:60px;">
    <span class="biaoti1">网 课 百 问 解 答</span>
     <span class="touxiang">

      <el-button @click="tuichu">返回类别</el-button>
    </span>
    
   
  </el-header>


  <el-container class="contain">
    <!-- <el-aside  class="aside" style="width:150px;"><asidess></asidess></el-aside> -->
       <!-- <router-view></router-view>   -->
       <el-collapse v-model="activeName" accordion style="width:700px; font-size:20px;margin-top: 60px;">
            <el-collapse-item title="1.直播教学时，网络不好，可能出现哪些现像。如：卡顿、黑屏、延迟等怎样解决？" name="1">
                <div style="color:rgb(177, 0, 0);">建议：使用有线网络最好，关闭电脑其他占内存软件。</div>
            </el-collapse-item>
            <el-collapse-item title="2.直播网络问题导致不能结束直播怎样解决？" name="2">
                <div style="color:rgb(177, 0, 0);">尝试退出钉钉后，再次重新登录进入</div>
                <img src="../assets/3_1.png" style="max-width:650px; max-height:300px;"/>
            </el-collapse-item>
            
        </el-collapse>


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