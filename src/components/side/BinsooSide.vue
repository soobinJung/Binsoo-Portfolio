<template>
  <div style="display: flex;">
     <div style="width: 500px; padding : 0 30px 0 30px; float:left; padding :20px 0 0 20px; border-radius:50px 0  0 50px; "> 
       <div style = "padding: 0 0 30px 0; text-align : left; cursor: pointer;">
           <span style="font-family: BMEULJIROTTF; font-size : 25px"> 자발적 개인 프로젝트 👩‍💻 </span>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(1)" @mouseout="progressStatusOut(1)" @click="changeCilck(1)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/> 따자 </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="80" :status="progressStatus1" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(2)" @mouseout="progressStatusOut(2)" @click="changeCilck(2)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/> 게시판 API MONGO </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="90" :status="progressStatus2" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(3)" @mouseout="progressStatusOut(3)" @click="changeCilck(3)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/> 게시판 API RDB</span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="90" :status="progressStatus3" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(4)" @mouseout="progressStatusOut(4)" @click="changeCilck(4)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/>  학습 관리 시스템 - LMS </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="90" :status="progressStatus4" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(5)" @mouseout="progressStatusOut(5)" @click="changeCilck(5)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/>  우리동네 동아리 </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="90" :status="progressStatus5" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(6)" @mouseout="progressStatusOut(6)" @click="changeCilck(6)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/>  웹소켓을 이용한 채팅 </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="90" :status="progressStatus6" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(7)" @mouseout="progressStatusOut(7)" @click="changeCilck(7)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/>  JWT 발급  </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="80" :status="progressStatus7" style = "margin : 10px 0 0 0; "/>
        </div>
      </div>
      <div style="width:950px; float:left; text-align:left; padding :110px 0 0 20px; margin : 0 20px 0 0; =border-radius:0 50px 50px 0;">
        <div style="border : 2px solid #67C23A; background : #d6ffc2; padding:50px; margin : 0 50px 0 0; border-radius:50px; font-family: BMYEONSUNG; font-size : 20px">
          <compo1 v-if = "componentIf === 1"/>
          <compo2 v-if = "componentIf === 2"/>
          <compo3 v-if = "componentIf === 3"/>
          <compo4 v-if = "componentIf === 4"/>
          <compo5 v-if = "componentIf === 5"/>
          <compo6 v-if = "componentIf === 6"/>
          <compo7 v-if = "componentIf === 7"/>
        </div>
      </div>
        <div style="width:350px; text-align : center; border-radius:50px; background : white; ; font-family: BMEULJIROTTF; color: white;">
          <div style=" height:50px; padding : 100px 0 30px 0">
            <div style="width:100%"><span style="font-size:25px; color :BLACK"> 피, 땀, 눈물같은 자격증 💦</span></div>
         </div>
          <div>
            
         <div style=" height:100px; padding : 20px 0 10px 0;">
            <div style="width:100%; padding : 0 0 20px 0"><span style="font-size:25px; color : BLACK"><i class="el-icon-circle-plus-outline"></i> 정보처리 기사</span></div>
            <div style="width:100%"><span style="font-size:20px; color :BLACK">2020.01.01 </span></div>
         </div>
         <div style=" height:100px; padding : 20px 0 10px 0">
            <div style="width:100%; padding : 0 0 20px 0"><span style="font-size:25px; color :BLACK"><i class="el-icon-circle-plus-outline"></i> 정보처리 산업기사</span></div>
            <div style="width:100%"><span style="font-size:20px; color :BLACK"> 2020.01.01 </span></div>
         </div>
         <div style=" height:100px; padding : 20px 0 10px 0">
            <div style="width:100%; padding : 0 0 20px 0"><span style="font-size:25px; color :BLACK"><i class="el-icon-circle-plus-outline"></i> 네트워크 관리사 2급</span></div>
            <div style="width:100%"><span style="font-size:20px; color :BLACK"> 2020.01.01 </span></div>
         </div>
         <div style=" height:100px; padding : 20px 0 10px 0">
            <div style="width:100%; padding : 0 0 20px 0"><span style="font-size:25px; color :BLACK"><i class="el-icon-circle-plus-outline"></i> 사회복지사 2급</span></div>
            <div style="width:100%"><span style="font-size:20px; color :BLACK"> 2020.01.01 </span></div>
         </div>
         <div style=" height:100px; padding : 20px 0 10px 0">
            <div style="width:100%; padding : 0 0 20px 0"><span style="font-size:25px; color :BLACK"><i class="el-icon-circle-plus-outline"></i> 운전면허증 2급</span></div>
            <div style="width:100%"><span style="font-size:20px; color :BLACK"> 2020.01.01 </span></div>
         </div>
          </div>
      </div>
  </div>
</template>

<script>
import compo1 from "./components/Side1.vue";
import compo2 from "./components/Side2.vue";
import compo3 from "./components/Side3.vue";
import compo4 from "./components/Side4.vue";
import compo5 from "./components/Side5.vue";
import compo6 from "./components/Side6.vue";
import compo7 from "./components/Side7.vue";

export default {

  name : 'Binsoo Side'
  , components : {
    compo1
    , compo2
    , compo3
    , compo4
    , compo5
    , compo6
    , compo7
  }
    , data () {
      return {
        skillMsg : ''
        , progressStatus0 : "success"
        , progressStatus1 : "success"
        , progressStatus2 : "success"
        , progressStatus3 : "success"
        , progressStatus4 : "success"
        , progressStatus5 : "success"
        , progressStatus6 : "success"
        , progressStatus7 : "success"
        , componentIf : 0

      }
    }
    , created () {
      this.changeCilck(1)
    }
    , methods : {
        changeCilck(value){
          this.componentIf = value
        }

        , progressStatusOver (index) {
          if(index === 0){
            this.progressStatus0 = ''
          }else if(index === 1){
            this.progressStatus1 = ''
          }else if(index === 2){
            this.progressStatus2 = ''
          }else if(index === 3){
            this.progressStatus3 = ''
          }else if(index === 4){
            this.progressStatus4 = ''
          }else if(index === 5){
            this.progressStatus5 = ''
          }else if(index === 6){
            this.progressStatus6 = ''
          }else if(index === 7){
            this.progressStatus7 = ''
          }else if(index === 8){
            this.progressStatus8 = ''
          }else if(index === 9){
            this.progressStatus9 = ''
          }else if(index === 10){
            this.progressStatus10 = ''
          }
          this.changeCilck (index)
        }

        , progressStatusOut (index) {
          if(index === 0){
            this.progressStatus0 = 'success'
          }else if(index === 1){
            this.progressStatus1 = 'success'
          }else if(index === 2){
            this.progressStatus2 = 'success'
          }else if(index === 3){
            this.progressStatus3 = 'success'
          }else if(index === 4){
            this.progressStatus4 = 'success'
          }else if(index === 5){
            this.progressStatus5 = 'success'
          }else if(index === 6){
            this.progressStatus6 = 'success'
          }else if(index === 7){
            this.progressStatus7 = 'success'
          }else if(index === 8){
            this.progressStatus8 = 'success'
          }else if(index === 9){
            this.progressStatus9 = 'success'
          }else if(index === 10){
            this.progressStatus10 = 'success'
          }
        }
        , windowOpen(url){
          window.open(url)
        }
    }
}
</script>

<style>

.jb-wrap {
	position: relative;
}
.jb-wrap img {
	width: 100%;
	vertical-align: middle;
}
.jb-text {
	padding: 5px 10px;
	background-color: yellow;
	text-align: center;
	position: absolute;
	top: 40%;
	left: 40%;
}
/* 
 .skill:hover {
  cursor: pointer;
  background-color: #7fd952;
  border-radius:10px;
  color: whitesmoke;
  padding: 30px;
} */


</style>