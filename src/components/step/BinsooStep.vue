<template>
  <div style="display:flex; justify-content:space-between; padding : 0 0 20px 10px; ">
    <div style=" width:80%;">
      <div style="height: 70px; margin : 30px 0 0 0; ">
        <el-steps :space="200" :active="active" simple>
          <el-step @click.native="changeCilck(1)" style="cursor: pointer;" title="휘경여중고" icon="el-icon-camera"/>
          <el-step @click.native="changeCilck(2)" style="cursor: pointer;" title="삼척시청 핸드볼팀" icon="el-icon-camera"/>
          <el-step @click.native="changeCilck(3)" style="cursor: pointer;" title="웹개발 교육" icon="el-icon-camera"/>
          <el-step @click.native="changeCilck(4)" style="cursor: pointer;" title="RSN" icon="el-icon-camera"/>
          <el-step @click.native="changeCilck(5)" style="cursor: pointer;" title="이직" icon="el-icon-camera"/>
        </el-steps>
      </div>
      <div style = "height:290px">
        <Step1 v-if="active === 1"/>
        <Step2 v-if="active === 2"/>
        <Step3 v-if="active === 3"/>
        <Step4 v-if="active === 4"/>
        <Step5 v-if="active === 5"/>
      </div>
    </div>
    <div style="width:20%; border:10px solid #e6e6e6; height:390px; margin : 30px 0 0 0; border-radius: 30px;">
      <img :src="path" width="377px" height="390px" style="border-radius: 20px;"/>
    </div>
  </div>
</template>

<script>

import Step1 from './components/Step1.vue'
import Step2 from './components/Step2.vue'
import Step3 from './components/Step3.vue'
import Step4 from './components/Step4.vue'
import Step5 from './components/Step5.vue'


export default {
  name: 'BinsooStep'
  
  , components: {
    Step1
    , Step2
    , Step3
    , Step4
    , Step5
  }

  , data () {
    return {
      active : 1
      , path : require("../../assets/step/step1.jpg")
    }
  }
   , methods : {
        changeCilck(value){
          this.active = value

          if(value === 1){
            this.path =  require("../../assets/step/step1.jpg")
          }else if(value === 2){
            this.path =  require("../../assets/step/step2.jpg")
          }else if(value === 3){
            this.path =  require("../../assets/step/step3.jpg")
          }else if(value === 4){
            this.path =  require("../../assets/step/step4.jpg")
          }else if(value === 5){
            this.path =  require("../../assets/step/step5.jpg")
          }
        }
    }


}
</script>

<style>

.yellowfont {
  background: linear-gradient(to top, #FFE400 50%, transparent 50%)
}

</style>