<template>
  <div style="display:flex; justify-content:space-between; background:#DDDDDD">
    <div style=" width:80%;">
      <div style="height: 70px; margin : 30px 0 0 0; ">
        <el-steps :space="200" :active="active" simple>
          <el-step @click.native="changeCilck(1)" title="휘경여중고" icon="el-icon-camera"/>
          <el-step @click.native="changeCilck(2)" title="삼척시청 핸드볼팀" icon="el-icon-camera"/>
          <el-step @click.native="changeCilck(3)" title="웹개발 국비교육" icon="el-icon-camera"/>
          <el-step @click.native="changeCilck(4)" title="웹개발 인턴교육" icon="el-icon-camera"/>
          <el-step @click.native="changeCilck(5)" title="RSN" icon="el-icon-camera"/>
        </el-steps>
      </div>
      <div style = "border:1px solid black; height:290px;">
        <Step1 v-if="active === 1"/>
        <Step2 v-if="active === 2"/>
        <Step3 v-if="active === 3"/>
        <Step4 v-if="active === 4"/>
        <Step5 v-if="active === 5"/>
      </div>
    </div>
    <div style="width:20%; border:1px solid red; height:390px;">

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
    }
  }
   , methods : {
        changeCilck(value){
          this.active = value
        }
    }


}
</script>

<style>

</style>