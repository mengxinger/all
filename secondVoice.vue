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
       <el-collapse v-model="activeName" accordion style="width:750px; font-size:20px;margin-top: 60px;">
            <el-collapse-item title="1.直播教学中有噪音是怎么回事？播电子书完全听不清怎样解决？？" name="1">
                <div style="color:rgb(177, 0, 0);">答：麦克风声音跟电脑本身声音互相干扰，要在直播音频设置里面，教师讲课时打开麦克风，关闭扬声器，播放视频时关闭麦克风，打开扬声器，这样就可以避免相互干扰，消除噪音。</div>
            </el-collapse-item>
            <el-collapse-item title="2.直播教学中的连线怎样使用，连麦声音小的原因是什么？" name="2">
                <div style="color:rgb(177, 0, 0);">
                  答： 发起直播时，发起人需要打开连麦功能，观看直播的用户才能申请连麦，直播过程中，观看直播用户点击连麦按钮即可申请连麦，直播发起人也可以主动连麦某个观看用户。<br/>
     连麦声音小的原因有以下几种：1.电脑音频设置中麦克风音量太小，或者设备电脑或者手机外放音量太小。2.直播中音频设置的麦克风音量或者直播以及观看设备音量太小。3.麦克风声音跟直播设备以及观看设备外放声音有干扰。
                </div>
            </el-collapse-item>
            <el-collapse-item title="3.在线课堂上课中，老师声音忽有忽无，设备检查没问题，笔记本上课时学生听到老师的声音很遥远，不清楚怎样解决？" name="3">
                <div style="color:rgb(177, 0, 0);">答：目前是全国网课高峰期，直播授课用户以及观看直播用户太多，容易造成网络拥堵，建议改用群直播模式进行授课，或者使用手机5G网络进行授课及观看。</div>
            </el-collapse-item>
            <el-collapse-item title="4.直播时能不能也看到全体学生的画面，怎样开启全体学生的麦克风？" name="4">
                <div style="color:rgb(177, 0, 0);">答：普通直播无法看到全体学生画面，也无法开启全体学生的麦克风，只有当学生申请连麦时才能使用麦克风。在线课堂模式下可以在直播画面右下方看到全体学生画面，画面下方有全员禁言按钮，可以设置强制全员禁言以及全员禁言（此禁言学生可以自动打开），还可以解除全员禁言。  </div>
            </el-collapse-item>
            <el-collapse-item title="5.耳机声音非常小，基本听不到，电脑麦开到最大（直播声音小怎样处理）？" name="5">
                <div style="color:rgb(177, 0, 0);">答：1.可能时观看设备问题，观看设备，设置扬声器音量调大，耳机音量调大。2.可能时网络问题，网络延迟及卡顿，退出重进。</div>
            </el-collapse-item>
            <el-collapse-item title="6.钉钉在线课堂两个班联播时声音有时出现卡顿怎样解决？" name="6">
                <div style="color:rgb(177, 0, 0);">答：首先直播设备建议使用电脑，尽量不要使用手机，电脑各方面性能更加稳定，并且尽量使用有线网络。如果是用手机直播，建议使用手机自带5G网络进行直播。</div>
            </el-collapse-item>
            <el-collapse-item title="7.直播中，孩子回答问题时有回音怎样解决？" name="7">
                <div style="color:rgb(177, 0, 0);">答：回音是麦克风声音跟电脑或者手机外放声音干扰造成的，可以让孩子把观看直播设备外放声音调小甚至关闭即可，只保留麦克风与老师交流。</div>
            </el-collapse-item>
            <el-collapse-item title="8.钉钉播电子书有电音，听不清怎样解决？" name="8">
                <div style="color:rgb(177, 0, 0);"> 答：直播页面左下角音频设置，关闭麦克风，保留例如扬声器等直播设备外放声音。</div>
            </el-collapse-item>
            <el-collapse-item title="9.直播时，笔记本外放视频，学生听不到声音怎样解决？" name="9">
                <div style="color:rgb(177, 0, 0);">答：播放电脑内的视频音频需要共享电脑音频，让主讲老师将声音设置里把扬声器声音选顷打开即可。</div>
            </el-collapse-item>
            <el-collapse-item title="10.视频会议中应怎么避免产生杂音？ " name="10">
                <div style="color:rgb(177, 0, 0);">答：在会议控制选项里设置全员静音，需要某位人员讲话时手动解除对应人员静音。</div>
            </el-collapse-item>
            <el-collapse-item title="11.腾讯会议播电子书完全听不清怎样解决？" name="11">
                <div style="color:rgb(177, 0, 0);">
                  答：播放电脑内的视频音频需要共享电脑音频，让主讲老师将声音设置里把扬声器声音选顷打开即可。<br/>
                  直播中的噪音可能是插着耳机，电脑同时又自带麦克风，产生了“双重声音”，通用直播下在声音设置中关闭一个麦克风。<br/>
                  直播时教师说话没声音请检查直播界面下方的【声音设置】/【设置】，查看麦克风是否点亮，音量是否调到最大。<br/>
                  声音小，可以尝试靠近耳机麦克风，或者退出课堂，重启一遍。
                </div>
                <img src="../assets/1_1.png" style="max-width:650px; max-height:300px;"/>

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
