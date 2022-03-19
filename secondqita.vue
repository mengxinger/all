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
            <el-collapse-item title="1.在线课堂如何使用？" name="1">
                <div style="color:rgb(177, 0, 0);">答：电脑端操作方式：【班级群界面】-【发起在线课堂】-点击添加需要上课的 学生。左侧是工具栏，供上课时需要使用。上课开始后，学生会被呼叫，点击接受则进入课堂开始上课。</div>
            </el-collapse-item>
            <el-collapse-item title="2.34.直播中的签到显示最长是二分钟，能不能更改时间？" name="2">
                <div style="color:rgb(177, 0, 0);">答：最长时间为5分钟,开启直播后在上方工具栏中,点击更多中签到在弹出的窗口中设置签到时长点击立即发起即可。</div>
                <img src="../assets/5_1.png" style="max-width:650px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="3.下课后显示还在会议中无法开新直播怎样解决？" name="3">
                <div style="color:rgb(177, 0, 0);">答：退出软件重新试试，检查有无结束全部直播</div>
            </el-collapse-item>
            <el-collapse-item title="4.视频会议的课堂模式无法保存回放？" name="4">
                <div style="color:rgb(177, 0, 0);">答：建议使用直播-课堂直播，可以进入前选择保存回放.</div>
                <img src="../assets/5_2.png" style="max-width:350px; max-height:400px;"/>
                <div style="color:rgb(177, 0, 0);">钉钉在线课堂也有回放功能，需要直播老师通过分享到群的方式进行保存回放。</div>
                <img src="../assets/5_3.png" style="max-width:350px; max-height:400px;"/>
            </el-collapse-item>
            <el-collapse-item title="5.系统盘满了怎样清理？" name="5">
                <div style="color:rgb(177, 0, 0);">答：系统盘满了后可通过腾讯管家或360管家清理，以腾讯管家为例，点击垃圾清理中的系统盘瘦身进行清理。</div>
                <img src="../assets/5_4.png" style="max-width:650px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="6.电脑经常弹窗怎样关闭？" name="6">
                <div style="color:rgb(177, 0, 0);">答：可下载腾讯管家软件，在腾讯管家软件工具箱中软件弹窗拦截功能开启软件弹窗拦截。</div>
                <img src="../assets/5_5.png" style="max-width:400px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="7.录制时抓取不到课堂互动信息框；发起直播—课堂直播，老师界面不显示学生摄像头。" name="7">
                <div style="color:rgb(177, 0, 0);">答：想要显示摄像头，可使用在线课堂直播功能。</div>
            </el-collapse-item>
            <el-collapse-item title="8.微信下载的课件找不到了，应该去手机哪里找？怎样把课件放到手机钉钉的直播上面？" name="8" >
                <div style="color:rgb(177, 0, 0);">答：先下载手机版wps，手机直播需要开始直播后开启屏幕共享，在微信中打开课件后点击右上角三点符号，在弹出的弹窗中点击选择其他应用，选择WPS office和电脑同样播放。</div>
                <img src="../assets/5_6.png" style="max-width:650px; max-height:600px;"/>
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