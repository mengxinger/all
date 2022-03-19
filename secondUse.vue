<template>
<div>
  <el-header class="biaoti" style="height:60px;">
    <span class="biaoti1">网 课 百 问 解 答</span>
     <span class="touxiang">
      <el-button @click="tuichu">返回类别</el-button>
    </span>
    
   
  </el-header>


  <el-container class="contain">
    <!-- <el-aside  class="aside" style="width:150px;"><asidess></asidess></el-aside> -->
       <!-- <router-view></router-view>   -->
       <div style="width:900px;   margin-top: 60px;">
       <el-collapse v-model="activeName" accordion >
            <el-collapse-item title="1.联播教学如何开展？" name="1">
                <div style="color:rgb(177, 0, 0);">答：在打开钉钉直播前，设置直播标题下方有一添加联播群图标，可添加其他群联播（通用直播模式），课堂直播模式或者在线课堂都可以通过点击【分享到群】的方式添加群联播。</div>
                <img src="../assets/2_1.png" style="max-width:650px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="2.直播教学中的白板功能如何使用？" name="2">
                <div style="color:rgb(177, 0, 0);">答：打开直播共享屏幕后，在上方有一工具栏开启直播后点击白板工具就可使用。</div>
                <img src="../assets/2_2.png" style="max-width:650px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="3.如何实现百人以上大班额学生在2一3分钟内完成钉钉或腾讯课堂签到？" name="3">
                <div style="color:rgb(177, 0, 0);">答：开启直播后在上方工具栏中点击更多中签到在弹出的窗口中设置签到时长点击立即发起即可。</div>
                <img src="../assets/2_3.png" style="max-width:650px; max-height:300px;"/>
                <img src="../assets/2_3_2.png" style="max-width:450px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="4.如何一上课就了解学生的上线率和学生注意力集中情况？" name="4">
                <div style="color:rgb(177, 0, 0);">答：开启直播后在互动面板中可观察观看人数了解学生的上线率。学生注意力集中问题可以通过不定时回复多提问的方式。</div>
                <img src="../assets/2_4.png" style="max-width:350px; max-height:400px;"/>
            </el-collapse-item>
            <el-collapse-item title="5.怎样制作微课？" name="5">
                <div style="color:rgb(177, 0, 0);">答：使用智慧云平台教学助手中微课通工具，智慧云平台校级管理员在上次微课录制任务中有具体的操作说明和安装包。</div>
                <!-- <img src="../assets/2_1.png" style="max-width:650px; max-height:300px;"/> -->
            </el-collapse-item>
            <el-collapse-item title="6.电脑在线课堂，如何准确无误的给举手的XX同学递粉笔？" name="6">
                <div style="color:rgb(177, 0, 0);">答：课堂直播模式下，学生上台发言后，直播老师把粉笔递给学生，学生在手机端可以板书。</div>
                <img src="../assets/2_5.png" style="max-width:400px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="7.上课时如何保证教师应用视频、PPT、板书等快速转换？" name="7">
                <div style="color:rgb(177, 0, 0);">答：可以上课前将需要的东西提前打开，切换界面时可使用快捷键ALT+TAB 实现快速切换。</div>
            </el-collapse-item>
            <el-collapse-item title="8.用插入课件的方式播课件，课件就不能出现原来的动画效果，用屏幕共享就不能看大部分操作按纽，孩子上课情况的画面也没有了怎样处理？（在线课堂直播）" name="8" style="inline-height:20px;">
                <div style="color:rgb(177, 0, 0);">在在线课堂中，使用共享窗口，仅共享自己的ppt（WPS或者Office），然后ppt不要选择放映，而是选择阅读视图，这样也可以放映动画效果。这样的话在上方可以看到操作按钮，并且旁边有小窗，当鼠标移到右边小窗位置时，选择最大化，这时老师可以看到黑板视图。
                因为仅共享的是ppt，所以学生此时还是只看到ppt的内容，看不到黑板。老师可以在这里看到与学生的互动消息，也可以与学生互动。学生可以点开视频和麦克风与老师交流。</div>
                <img src="../assets/2_6.png" style="max-width:650px; max-height:300px;"/>
            </el-collapse-item>
            <el-collapse-item title="9.播放ppt时，要想与同学连麦需要先退出放映有没有更好地方法？" name="9">
                <div style="color:rgb(177, 0, 0);">答：可以不用全屏放映ppt，设置阅读模式放映，调整窗口大小，打开互动面板，即可讲课过程中和学生连线</div>
            </el-collapse-item>
            <el-collapse-item title="10.（手机当作摄像头使用）想用手机“发起直播”，手机拍摄老师在黑板上板演，但是老师如何从电脑端既能看到自己的课件展示、又能看到自己在屏幕里的样子？（多个屏幕共同显示）" name="10">
                <div style="color:rgb(177, 0, 0);">答：用两个账号分别登录电脑和手机，用电脑开启直播后手机账号也进入直播并邀请连麦，手机开启摄像头拍摄教师黑板讲解，电脑共享课件。（切勿忘记两个麦克风不能同时开启，只能开启一个设备的麦克风）。</div>
            </el-collapse-item>
            <el-collapse-item title="11.如何更便捷 让领导、教研员或同学科其他老师随时进入网课巡课、观课？（目前进网课看课程序太繁琐！）" name="11">
                <div style="color:rgb(177, 0, 0);">答：建议将教研员拉入班级群内，在线进行网上巡课</div>
            </el-collapse-item>
            <el-collapse-item title="12.应用什么软件可对学生以及上课教师的每节课（每一天）的网课表现，自动量化打分？" name="12">
                <div style="color:rgb(177, 0, 0);">答：推荐下载鸿合教学软件 鸿合π教学软件中的班级评价不错.</div>
            </el-collapse-item>
            
        </el-collapse>
       </div>

  </el-container>
</div>
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