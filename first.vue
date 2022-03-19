<template>

    <div class="login-container">
        <el-header class="biaoti" >
            <span class="biaoti1">网 课 百 问 解 答</span>
            
        
        </el-header>

        <div class="xia">

              <div>
                <div class="a_1" style="" @click="ToSecondUse">
                    功能问题
                </div>
                <div class="a_2" style="" @click="ToSecondVoice">
                    声音使用
                </div>
              </div>
              <div>
                <div class="a_2" style="" @click="ToSecondInter">
                    网络问题
                </div>
                <div class="a_1" style="" @click="ToSecondhudong">
                    师生互动问题
                </div>
              </div>
              <div>
                <div class="a_1" style="" @click="ToSecond">
                    相关问题视频教程
                </div>
                <div class="a_2" style="" @click="ToSecondqita">
                    其他分类
                </div>
              </div>
          
        </div>

       
          
    </div>
</template>

<script>

  export default {
    data() {
      return {
        
      }
    },
    methods: {
      ToSecondUse(){
          this.$router.push('/secondUse');   
      },
      ToSecondVoice(){
          this.$router.push('/secondVoice');   
      },
      ToSecondInter(){
          this.$router.push('/secondInter');   
      },
      ToSecondhudong(){
          this.$router.push('/secondhudong');   
      },
      ToSecondqita(){
          this.$router.push('/secondqita');   
      },
      ToSecond(){
          this.$router.push('/second');   
      }
    }
  }
</script>
<style>

.login-title{
    color:rgb(2, 41, 92);
    font-size: 47px;
    font-weight: 500;
    text-align: center;
    margin-top: 40px;
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
  /* color: #ffcf4bf1; */
  color: #f5c174;
  /* color:rgb(241, 216, 217); */
  font-family:'微软雅黑', Times, serif;
}

.login-container{
    position:absolute;
    width:100%;
    height:100%;
    /* background:url("../assets/denglu_back.jpeg") no-repeat; */
    background-size: 100% 100%;
}
.xia{
    margin: auto;
    text-align: center;
    width: 60%;
     margin-top: 85px;
}

.a_1{
    width: 300px;
    height: 120px;
    border: 1px;
    border-radius: 30px;
    display: inline-block;
    margin:5px;
    /* background:url("../assets/1.png"); */
    font-size: 30px;
    text-align: center;
    padding-top: 60px;
  font-family:'微软雅黑', Times, serif;

    /* background: rgb(50, 47, 102); */
    /* background: #8AB2A7; */
    background: #f5c174;
    color: #456481;
}
.a_2{
    width: 200px;
    height: 120px; 
    border: 1px;
    border-radius: 30px;
    display: inline-block;
    margin:5px;
    background:url("../assets/2.png");
    font-size: 30px;
    text-align: center;
  font-family:'微软雅黑', Times, serif;

    padding-top:60px;
    /* background: #cc7152; */
    background: #4e6f8d;
    color: #ffcf4bf1;


    /* background: rgb(167, 121, 22); */
}
/* .a_12{
    width: 520px;
    height: 100px;
    border: 1px;
    border-radius: 30px;
    
    background: #d3b778;
    display: inline-block;
    font-size: 30px;
    text-align: center;
  font-family:'微软雅黑', Times, serif;

    padding-top:60px;
    margin-top: 10px;
} */
/* background: rgba(102, 160, 97, 0.842); */
    /* background:url("../assets/12.png"); */
</style>
