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
            <el-collapse-item title="1.直播互动窗口连麦以后，互动窗口就变大了，变不回去，无法边讲课边看互动怎样解决？" name="1">
                <div style="color:rgb(177, 0, 0);">答：此问题在通用直播内无法解决，若有此需求建议不使用通用直播，使用在线课堂直播。</div>
            </el-collapse-item>
            <el-collapse-item title="2.直播时共享屏幕，无法点击看到学生的连麦要求，无法互动怎样解决？" name="2">
                <div style="color:rgb(177, 0, 0);">答：通用直播下，可以在电脑屏幕中间正上方打开工具窗口里的互动面板，拖到桌面一侧，实时查看学生上麦需求。</div>
                <img src="../assets/4_1.png" style="max-width:550px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="3.共享屏幕时播放的视频学生看不到，课件放映全屏也无法点击学生回答问题？" name="3">
                <div style="color:rgb(177, 0, 0);">答：1.可能仅共享了窗口可采用屏幕分享的方式共享整个屏幕再打开视频。</div>
                <img src="../assets/4_2.png" style="max-width:450px; max-height:300px;"/>
                <div style="color:rgb(177, 0, 0);">答：2.可将视频嵌入到ppt中。课件不要选择放映，而是选择阅读视图，这样即可全屏放映也可查看学生互动消息。（也可电脑开直播，手机打开钉钉观察学生互动消息。）</div>
                <img src="../assets/4_2_2.png" style="max-width:650px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="4.在线课堂，播放ppt时，找不到学生互动悬浮窗口？" name="4">
                <div style="color:rgb(177, 0, 0);">答：课件不要选择放映，而是选择阅读视图，这样即可全屏放映也可查看学生互动消息。（也可电脑开直播，手机打开钉钉观察学生互动消息。）</div>
                <img src="../assets/4_2_2.png" style="max-width:650px; max-height:300px;"/>

            </el-collapse-item>
            <el-collapse-item title="5.无法让学生连线？" name="5">
                <div style="color:rgb(177, 0, 0);">答：通用直播下，可以在电脑屏幕中间正上方打开工具窗口里的互动面板，拖到桌面一侧，实时查看学生上麦需求。</div>
                <img src="../assets/4_1.png" style="max-width:550px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="6.钉钉在线课堂，屏幕共享时如何实现与学生互动？" name="6">
                <div style="color:rgb(177, 0, 0);">答1：当鼠标移到右边小窗位置时，选择最大化，这时老师可以看到黑板视图。因为仅共享的是ppt，所以学生此时还是只看到ppt的内容，看不到黑板。老师可以在这里看到与学生的互动消息，也可以与学生互动。学生可以点开视频和麦克风与老师交流。</div>
                <img src="../assets/4_5.png" style="max-width:400px; max-height:300px;"/>
                <div style="color:rgb(177, 0, 0);">答2：界面底下会有互动消息模块，打开即可查看学生文字消息。</div>
                <img src="../assets/4_6.png" style="max-width:400px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="7.有时只能用群直播，无法举手怎样解决？" name="7">
                <div style="color:rgb(177, 0, 0);">答：通用直播状态下学生可以申请连麦</div>
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