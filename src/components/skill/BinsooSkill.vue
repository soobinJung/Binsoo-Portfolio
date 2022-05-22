<template>
  <div style="display: flex;">
     <div style="width: 500px; padding : 0 30px 0 30px; float:left; padding :20px 0 0 20px; border-radius:50px 0  0 50px; "> 
       <div style = "padding: 0 0 30px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(0)" @mouseout="progressStatusOut(0)" @click="changeCilck(0)">
           <span style="font-family: BMEULJIROTTF; font-size : 25px"> 이런 개발을 해왔어요 👩‍💻 </span>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(0)" @mouseout="progressStatusOut(0)" @click="changeCilck(0)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/> Rest API</span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="80" :status="progressStatus0" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(1)" @mouseout="progressStatusOut(1)" @click="changeCilck(1)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/> Spring boot </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="80" :status="progressStatus1" style = "margin : 10px 0 0 0; "/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(8)" @mouseout="progressStatusOut(8)" @click="changeCilck(8)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/> Git </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="30" :status="progressStatus8" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(9)" @mouseout="progressStatusOut(9)" @click="changeCilck(9)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/> Query 속도 개선</span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="30" :status="progressStatus9" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(10)" @mouseout="progressStatusOut(10)" @click="changeCilck(10)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/> 개발 / 운영 DB 분리 </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="50" :status="progressStatus10" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(4)" @mouseout="progressStatusOut(4)" @click="changeCilck(4)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/>  Cron </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="90" :status="progressStatus4" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(7)" @mouseout="progressStatusOut(7)" @click="changeCilck(7)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/> Crawling </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="70" :status="progressStatus7" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(11)" @mouseout="progressStatusOut(11)" @click="changeCilck(11)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/> Cros 해결 </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="70" :status="progressStatus11" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(2)" @mouseout="progressStatusOut(2)" @click="changeCilck(2)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/>  Mail </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="90" :status="progressStatus2" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(3)" @mouseout="progressStatusOut(3)" @click="changeCilck(3)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/>  Excel </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="90" :status="progressStatus3" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(5)" @mouseout="progressStatusOut(5)" @click="changeCilck(5)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/>  Vue Js </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="90" :status="progressStatus5" style = "margin : 10px 0 0 0"/>
        </div>
        <div style = "padding: 0 0 10px 0; text-align : left; cursor: pointer;" @mouseover="progressStatusOver(6)" @mouseout="progressStatusOut(6)" @click="changeCilck(6)">
          <span style="font-family: BMEULJIROTTF;"><i class="el-icon-caret-right"/>  Daemon </span>
          <el-progress :text-inside="true" :stroke-width="26" :percentage="80" :status="progressStatus6" style = "margin : 10px 0 0 0"/>
        </div>
      </div>
             
      <div style="width:950px; float:left; text-align:left; padding :110px 0 0 20px; margin : 0 20px 0 0; border-radius:0 50px 50px 0;">
        <div style="border : 2px solid #67C23A; background : #d6ffc2; padding:50px; margin : 0 50px 0 0; border-radius:50px">
          <span style="font-family: BMYEONSUNG; font-size : 20px;" v-html="skillMsg"/>
        </div>
      </div>

      <div style="width:350px; text-align : center; border-radius:50px; background : white; ; font-family: BMEULJIROTTF; color: white;">
         <div style=" height:100px; padding : 20px 0 10px 0;">
            <div style="width:100%; padding : 0 0 20px 0"><span class="yellowfont" style="font-size:25px; color : BLACK"> 이름 </span></div>
            <div style="width:100%"><span style="font-size:20px; color :BLACK"> 정수빈 / soobin Jung </span></div>
         </div>
        <div style=" height:100px; padding : 20px 0 10px 0;">
            <div style="width:100%; padding : 0 0 20px 0"><span class="yellowfont" style="font-size:25px; color : BLACK"> 나이 </span></div>
            <div style="width:100%"><span style="font-size:20px; color :BLACK"> 26살 </span></div>
         </div>
                  <div style=" height:100px; padding : 20px 0 10px 0;">
            <div style="width:100%; padding : 0 0 20px 0"><span class="yellowfont" style="font-size:25px; color : BLACK"> 연락처 </span></div>
            <div style="width:100%"><span style="font-size:20px; color :BLACK"> 010 8478 6861 </span></div>
         </div>
         <div style=" height:100px; padding : 20px 0 10px 0">
            <div style="width:100%; padding : 0 0 20px 0"><span class="yellowfont" style="font-size:25px; color :BLACK"> 주소 </span></div>
            <div style="width:100%"><span style="font-size:20px; color :BLACK"> 서울시 강서구 화곡동 까치산역 5분 거리 </span></div>
         </div>
         <div style=" height:100px; padding : 20px 0 10px 0">
            <div style="width:100%; padding : 0 0 20px 0"><span class="yellowfont" style="font-size:25px; color :BLACK">MBTI </span></div>
            <div style="width:100%"><span style="font-size:20px; color :BLACK"> ENFJ </span></div>
         </div>

      </div>
  </div>
</template>

<script>
export default {
  name : 'Binsoo Skill'
    , data () {
      return {
        skillMsg : ''
        , blogStatus : true
        , gitStatus  : true
        , progressStatus0 : "success"
        , progressStatus1 : "success"
        , progressStatus2 : "success"
        , progressStatus3 : "success"
        , progressStatus4 : "success"
        , progressStatus5 : "success"
        , progressStatus6 : "success"
        , progressStatus7 : "success"
        , progressStatus8 : "success"
        , progressStatus9 : "success"
        , progressStatus10 : "success"
        , progressStatus11 : "success"
        , vueImg : require("../../assets/lang/vue.jpg")
      }
    }
    , created () {
      this.changeCilck(5)
    }
    , methods : {
        changeCilck(value){

          if(Number(value) === 0){
            this.skillMsg = 
             `<span style = 'font-size:30px;'>REST API 설계</span><br><hr/><br>
            <i class="el-icon-caret-right"/></i> 코드 관리 REST API 개발 <br><br>
            <div style = 'font-size:18px; line-height : 30px'>
            기존에 RSET API 를 사용하지 않다가 REST API 를 도입을 시도하니 
            저와  팀원들이 REST API 에 대해 생소해하던 기억이 납니다. <br>
            인터넷에서 정보를 찾고 서점에가 관련 책도 구입하여 저희팀에 REST API 를 성공적으로 도입하려 애썼던 했던 기억이납니다.<br><br>
            <span class='yellowfont'>'REST API 는 명확하게 한가지일만 한다'</span> 라는 소신을 지키려 애썼고 
            그로인해 다양한 정보를 한번에 원하는 웹 사이트와의 충돌이 일어난 적이 많지만 
            그때마다 <span class='gubul'>지금 당장의 편의성보다는 앞으로 제 API 를 사용할 개발자를 생각하며 REST API 에 대한 제 소신을 잃지 않으려 공부하고 고민</span>했던 기억이 납니다.
          </div>    

            <br><br>
            <div style = 'font-size:15px'>
            - GET <br><br>
            /common/code?searchoption=codegroup&searchvalue=department <br>
            /common/code?searchoption=codedepth&searchvalue=1 <br><br>
            - POST <br><br>
            /common/code?codegroup=department&codevalue=A&codedepth=1&codepseq=23 <br><br>
            - PATCH <br><br>
            /common/code/{codeseq}?codegroup=news&codedepth=1 <br><br>
            - DELETE <br><br>
            /common/code/{codeseq} <br><br>
            </div>
            `

          }else if(Number(value) === 1){
            this.skillMsg = 
            `
            <div style = 'padding : 0 0 0 0px'>
              <span style = 'font-size:30px;'> Spring Dependency 활용 </span><br><hr/><br>
              <div style = 'font-size:18px; '>보통 프로젝트 설정시 초기 설정후에 변경은 드문일입니다. 다양한 Dependency를 활용하고자 노력했습니다.<br><br> </div>
              <div style = 'padding : 0px 0 30px 0'><span> <i class="el-icon-caret-right"/></i> 아래와 같은 Dependency 로 프로젝트를 세팅하여 개발을 하였습니다. </span></div>
             <div style = 'padding : 0 0 0 0'>
                <div style = 'display: flex; justify-content: left;'>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> Spring Web </h3>
                    </div>                  
                  </div>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> Spring Web Service </h3>
                    </div>                  
                  </div>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> Servlet </h3>
                    </div>                  
                  </div>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> - </h3>
                    </div>                  
                  </div>
                </div>
                <div style = 'display: flex; justify-content: left;'>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> Spring Data JPA </h3>
                    </div>                  
                  </div>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> Spring MongoDB </h3>
                    </div>                  
                  </div>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> MyBatis Framework </h3>
                    </div>                  
                  </div>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> MySQL Driver </h3>
                    </div>                  
                  </div>
                </div>
                <div style = 'display: flex; justify-content: left;'>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> Spring Security </h3>
                    </div>                  
                  </div>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> Lombok </h3>
                    </div>                  
                  </div>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> Jwt </h3>
                    </div>                  
                  </div>
                  <div style = 'border : 1px solid #edf3ff; width:25% ;height :180px; text-align : center;'>
                    <div style = 'padding : 48px 0 0 0' >
                      <h3> JUnit </h3>
                    </div>                  
                  </div>
                </div>
              </div>
            </div>
            `
          }else if(Number(value) === 2){
            this.skillMsg = 
            `
            <div style = 'padding : 0 0 0 0px'>
              <span style = 'font-size:30px;'> 메일 전송 </span><br><hr/><br>
                <div style = 'display: flex; justify-content: left; padding : 20px 0 0 0'>
                <span>
                  <i class="el-icon-caret-right"/></i> 메일 전송 개발 경험이 있습니다
                <span>
                <ol type="I">
                  <li style = 'padding : 10px 0 10px 0'>
                    고객사의 웹 사용량을 <span class='one'>EXCEL</span> 로 생성해 메일 정기발송
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    로그인 기능 중 비밀번호 재발급시 <span class='one'>HTML</span> 메일 발송
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    LMS 사이드 프로젝트에서 학생 <span class='one'>PDF</span> 이력서 기업에 메일 발송
                  </li>
                </ol>
              </div>
              </div>
            </div>
            `
          }else if(Number(value) === 3){
            this.skillMsg = 
            `
            <div style = 'padding : 0 0 0 0px'>
              <span style = 'font-size:30px;'> 액셀 파일 생성 </span><br><hr/><br>
                <div style = 'display: flex; justify-content: left; padding : 20px 0 0 0'>
                <span>
                  <i class="el-icon-caret-right"/></i> org.apache.poi 라이브러리 활용
                <span>
                <ol type="I">
                  <li style = 'padding : 10px 0 10px 0'>
                    빅데이터를 다루는 회사 특성상 액셀 다운로드 개발 경험이 많습니다
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    CellStyle 활용하여 액셀 디자인 가능합니다 
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    고객사마다 다른 액셀 유형를 원하는 상황이 잦아 유동적인 액셀 유형 선택이 가능하도록 설계 경험이 있습니다.
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    xml, xlsx, csv 파일 확장자를 다룰 수 있습니다.
                  </li>
                </ol>
              </div>
              </div>
            </div>
            `
          }else if(Number(value) === 4){
            this.skillMsg = 
            `
            <div style = 'padding : 0 0 0 0px'>
              <span style = 'font-size:30px;'> Cron 을 활용해서 웹 트래픽 분산처리하기 </span><br><hr/><br>
              <div style = 'padding : 0 0 0 0'>
                <div style = 'padding : 0px 0 10px 0'><span> <i class="el-icon-caret-right"/></i> cron 활용전 </span></div>
                <div style = 'padding : 0 0 30px 0'>
                  <span>
                    사용자가 업로드한 파일을 그때 그때 처리하기에는 상당한 비용이 들어 <span class='gubul'>빠른 응답이 이루워지지 못했습니다</span>.
                  </span>
                </div>

                <div style = 'display: flex; justify-content: left;'>
                  <div style = 'width:33% ;height :120px; text-align : center;'>
                    <div style = 'padding : 0 0 0 0' >
                      <h3> 사용자 대용량 </h3>
                      <h3> 엑셀 파일 업로드 </h3>
                    </div>                  
                  </div>
                  <div style = 'width:33% ;height :120px; text-align : center;'>
                    <div style = 'padding : 28px 0 0 0' >
                      <h3> -> </h3>
                    </div>                  
                  </div>
                  <div style = 'width:33% ;height :120px; text-align : center;'>
                    <div style = 'padding : 0 0 0 0' >
                      <h3>대용량 액셀 읽고 저장하기까지 </h3>
                      <h3> 많은 시간이 소요 </h3>
                    </div>                  
                  </div>
                </div>
                
                <div style = 'padding : 50px 0 10px 0'><span> <i class="el-icon-caret-right"/></i> cron 활용 </span></div>
                <div style = 'padding : 0 0 30px 0'>
                  <span>
                    사용자가 업로드한 파일을 서버에 저장 후 크론을 활용해 30초 주기로 데몬 실행을 실행시킨 후 <br> 액셀 파일을 처리하여 <span class='yellowfont'>웹 서버의 부하를 <span class='one'>분산</span></span>시켰습니다.
                  </span>
                </div>
                <div style = 'padding : 0 0 0 0'>
                <div style = 'display: flex; justify-content: left;'>
                  <div style = 'width:33% ;height :120px; text-align : center;'>
                    <div style = 'padding : 0 0 0 0' >
                      <h3> 30 초 주기 </h3>
                      <h3> 데몬 실행 </h3>
                    </div>                  
                  </div>
                  <div style = 'width:33% ;height :120px; text-align : center;'>
                    <div style = 'padding : 28px 0 0 0' >
                      <h3> -> </h3>
                    </div>                  
                  </div>
                  <div style = 'width:33% ;height :120px; text-align : center;'>
                    <div style = 'padding : 25px 0 0 0' >
                      <h3> 대용량 액셀처리 </h3>
                    </div>                  
                  </div>
                </div>
            </div>
            `
          }else if(Number(value) === 5){
            this.skillMsg = 
            `
            <div style = 'padding : 0 0 0 0px; class = 'vue-back'>
              <span style = 'font-size:30px;'> Vue js 활용 </span><br><hr/><br>
              <div style = 'display: flex; justify-content: left; padding : 0 0 0 0'>
                <span>
                  <i class="el-icon-caret-right"/></i>  Vue Life Cycle
                <span>
                <ol type="I">
                  <li style = 'padding : 10px 0 10px 0'>
                    Vue 를 이용해 API 를 호출하고 화면을 세팅하며 Vue Life Cycle 을 익혔습니다.
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    Vue Life Cycle 을 활용해서 불필요한 API 호출을 제거하였습니다.
                  </li>
                </ol>
              </div>
              <div style = 'display: flex; justify-content: left; padding : 20px 0 0 0'>
                <span>
                  <i class="el-icon-caret-right"/></i>  Vuex
                <span>
                <ol type="I">
                  <li style = 'padding : 10px 0 10px 0'>
                    Store 를 활용해 전역적으로 관리가 필요한 데이터를 관리하여 컴포턴트간의 소통을 원활히 하였습니다.
                  </li>
                </ol>
              </div>
              <div style = 'display: flex; justify-content: left; padding : 20px 0 0 0'>
                <span>
                  <i class="el-icon-caret-right"/></i>  컴포넌트간의 소통 
                <span>
                <ol type="I">
                  <li style = 'padding : 10px 0 10px 0'>
                    props 과 emit 을 이용해서 컴포넌트간의 소통을 원활히 하였습니다.
                  </li>
                </ol>
              </div>
              
            </div>
            `
          }else if(Number(value) === 6){
            this.skillMsg = 
            `
           <div style = 'padding : 0 0 0 0px'>
              <span style = 'font-size:30px;'> 데몬 개발하기 </span><br><hr/><br>
              <div style = 'display: flex; justify-content: left; padding : 0 0 0 0'>
                <span>
                  <i class="el-icon-caret-right"/></i> 사람이 주기적으로 해줘야 하는 수동적으로 해야하는 일을 데몬으로 자동화 시킬 수 있는일에 
                  <br> &nbsp &nbsp  굉장히 흥미를 느끼는 중입니다 : )
                <span>
                <ol type="I">
                  <li style = 'padding : 10px 0 10px 0'>
                    매달 서비스 사용량을 원하는 날에 메일 💌 로 보고하는 데몬 개발 경험
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    서버에 업로드 된 데이터 가공 후 db 에 저장해주는 데몬 개발 경험
                  </li>
                </ol>
              </div> 
            </div>
            `
          }else if(Number(value) === 7){
            this.skillMsg = 
            `
            <div style = 'padding : 0 0 0 0px'>
              <span style = 'font-size:30px;'> Naver 사전 뜻 크롤링 </span><br><hr/><br>
                <div style = 'display: flex; justify-content: left; padding : 20px 0 20px 0'>
                <span>
                  <i class="el-icon-caret-right"/></i> 대용량의 단어를 하나씩 수작업으로 검색 후 뜻을 옮겨적는 업무가 있었습니다. <br> &nbsp &nbsp &nbsp 수작업을 대신하기 위한 크롤링을 개발하여 업무에 적용했습니다.
                <span>
                <ol type="I">
                  <li style = 'padding : 10px 0 10px 0'>
                    액셀 파일에 있는 단어 데이터들을 단어검색 URL 에 조합후 NAVER API 를 호출
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    응답 결과가 html 로 반환되면 특정 태그를 기준으로 단어의 검색 결과의 시작과 끝을 찾아낸다
                  </li>
                </ol>
              </div>
              </div>
                <div style = 'display: flex; justify-content: left; width : 800px; height : 100px;'>
                  <div style = 'width : 33%; text-align : center; padding : 30px 0 0 0; font-size:50px'> ↗   </div>
                  <div style = 'width : 33%; text-align : center; padding : 0 0 60px 0; font-size:25px'>API 호출</div>
                  <div style = 'width : 33%; text-align : center; padding : 30px 0 0 0; font-size:50px'>↘</div>
                </div>
                <div style = 'display: flex; justify-content: left; width : 800px; height : 100px;'>
                  <div style = 'width : 33%; text-align : center; padding : 30px 0 0 0; font-size:25px'> naver.com?word=단어 </div>
                  <div style = 'width : 33%; text-align : center'> </div>
                  <div style = 'width : 33%; text-align : center; padding : 30px 0 0 0; font-size:25px'>검색 결과 반환</div>
                </div>
                <div style = 'display: flex; justify-content: left; width : 800px; height : 100px; padding : 0 0 70px 0'>
                  <div style = 'width : 33%; text-align : center; font-size:50px'>↖</div>
                  <div style = 'width : 33%; text-align : center; padding : 60px 0 0 0'> <span style = 'font-size:25px'>응답 결과 정제 <br></span> <br> nsfdkjnalnals<span style = 'color : red'><시작> <br></span>afsnhnascnjksjanciuasvinaskn<span style = 'color : red'> <br><끝></span>dsfjdaobgoiuadbgoasf </div>
                  <div style = 'width : 33%; text-align : center; font-size:50px'>↙</div>
                </div>
            </div>
            `
          }else if(Number(value) === 8){
            this.skillMsg = 
            `
            <div style = 'padding : 0 0 0 0px'>
              <span style = 'font-size:30px;'> SVN 을 사용하던 Team, Gitlab 도입하다 </span><br><hr/><br>
              <div style = 'display: flex; justify-content: left; padding : 0 0 0 0'>
                <div style = 'font-size : 18px'>
                  저희 팀은 기존에 SVN 으로 코드 병합을 했었지만 Gitlab 을 도입 후 대부분의 팀원들이 Git 사용법에 미숙하여 GitLab 을 활용하기까지 어려움이 있었습니다.<br> <br> 
                <div>
                <span>
                  <i class="el-icon-caret-right"/></i> 저는 원활한 소통을 위해 아래와 같은 메뉴얼을 작성하여 공유하였습니다. 
                <span>

                <div style = "float:left; padding : 50px; width : 100%">
                  <a href="https://foremost-taxi-c21.notion.site/2deb0e2c235d43e592c2cbb46c6d068b?v=c5bec0c20e954d2d96996833b3669efd">
                    <div class = 'gitatag' style = "float:left; padding : 50px 70px; font-size : 45px; margin : 0 60px 0 0;  border : 1px solid black;" on-click:"windowOpen()">
                      Git 사용법
                    </div>
                  </a>
                  <a href="https://foremost-taxi-c21.notion.site/7854d30eb8594bce8cb5bc8db5978af9?v=d34e0147f5da40b79aa9b587b30d5f42">
                    <div class = 'gitatag' style = "float:left; padding : 50px 70px; font-size : 45px; border : 1px solid black">
                      Git 컨벤션
                    </div>
                  </a>
                </div>
                <div style = "width : 100%">
                <span>
                  <i class="el-icon-caret-right"/></i>  변화 1
                <span>
                <ol type="I">
                  <li style = 'padding :7px'>
                    덕분에 깃에 접근하기 쉬워졌다며 칭찬을 무진장 받아서 회사생활에 힘이 났습니다. (불끈)
                  </li>
                  <li style = 'padding :7px'>
                    타부서에서도 제 문서를 요청해 또 한번 힘이 났습니다. (불끈 불끈)
                  </li>
                  <li style = 'padding :7px'>
                    기존에는 어수선했던 업무할당이 이슈 할당으로 일의 우선순위가 명확해졌습니다.
                  </li>
                  <li style = 'padding :7px'>
                    신규 개발건시 위키를 통해 문서화를 진행하여 타부서에서 API 문의가 들어왔을 때 위키링크를 공유하여 원활한 정보 공유가 이루어졌습니다.
                  </li>
                  <li style = 'padding :7px'>
                    브랜치를 이용해 여러가지 개발을 구분지어 동시에 진행할 수 있었습니다.
                  </li>
                </ol>
              </div>
              </div>
            </div>
            `
          }else if(Number(value) === 9){
            this.skillMsg = 
            `
            <div style = 'padding : 0 0 0 0px'>
              <span style = 'font-size:30px;'> 15만건 데이터에서 5건 데이터 가져오는데 4초라니 ,, </span><br><hr/><br>
              <div style = 'display: flex; justify-content: left; padding : 0 0 0 0'>
                <span>
                  빅데이터 플랫폼 회사에서 일하다보니 대용량 데이터를 다루는 일이 흔한일이 되어버렸습니다.<br>
                <span>
                <span>
                 하지만 데이터를 로딩하는데 4초가 걸리는 상황이 발생했고 쿼리 소요시간 단축을 해야했습니다 <br> 
                <span>
                <span>
                  4초에서 0.59초까지 단축을 했고 단축을 하기까지 하루가 꼬박걸렸습니다.<br> <br> 
                <span>
                 <span>
                  <i class="el-icon-caret-right"/></i> 내가 생각한 기존 쿼리의 문제점
                <span>
                <ol>
                  <li style = 'padding : 10px 0 10px 0'>
                    처음 필터링이 시작되는 쿼리가 Limit 이 되기도 전에 필요없는 조인이 이루어지고 있었습니다. 
                      <ol>
                        <li  style = 'padding : 10px 0 10px 0'>
                          사용할 데이터는 5건인데 <span class='gubul' style = 'line-height : 50px'>15만건의 데이터를 조인</span>하고 있어 느렸습니다.
                        </li>
                        <li  style = 'padding : 5px 0 10px 0'>
                          메인 테이블에서 조건에 맞는 <span class='yellowfont'><span class='one'>5건만</span> 필터링 후 하나의 서브 테이블을 구성</span>하고 5건의 데이터를  <br> 연관테이블과 조인을 하니 속도가 눈에 띄게 개선되었습니다.
                        </li>
                      </ol>
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    매번 같은 결과를 반환하는 서브 쿼리를 구성하여 테이블 생성하여 사용하였는데 <span class='gubul' style = 'line-height : 50px'>매 행마다 서브 테이블을 구성</span>하니 속도가 현저히 낮았습니다.
                    <ol>
                        <li  style = 'padding : 10px 0 10px 0'>
                          쿼리를 분리시켰습니다. 기존 서브 테이블의 값을 쿼리 던지기 전에 구해와 <span class='yellowfont'>서브테이블을 <span class='one'>제거</span></span>했습니다.
                        </li>
                        <li  style = 'padding : 5px 0 10px 0'>
                          이 로직을 변경하니 2초가 개선되었습니다.
                        </li>
                      </ol>
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    IN 절을 EXISTS 로 변경하였습니다.
                    <ol>
                        <li  style = 'padding : 10px 0 10px 0'>
                          위에서 구해온 데이터로 in 절을 사옹하여 필터링 했었는데 <span class='yellowfont'><span class='one'>EXISTS</span>로 변경</span>하니 1초의 속도가 향상되었습니다.
                        </li>
                      </ol>
                  </li>
                </ol>
              </div>
            </div>
            `
          }else if(Number(value) === 10){
            this.skillMsg = 
            `
            <div style = 'padding : 0 0 0 0px'>
              <span style = 'font-size:30px;'> 개발 DB 운영 DB 분리 시켜 관리하세요 ! </span><br><hr/><br>
              <div style = 'display: flex; justify-content: left; padding : 0 0 0 0'>
                <span>
                  웹 사이트를 개발/운영 사이트로 나누어 개발할 예정이었습니다.<br> 
                  차장님께서는 배포시마다 매번 mybatis 폴더를 두 개로 관리하라고 하셨고,, <br>  프로젝트에 투입되는 개발자가 매번 바뀌는 상황에 그런 관리는 힘들다고 판단했습니다 (유지보수 비용,, 3배ㅠㅠ)<br> <br> 
                <span>
                 <span>
                  <i class="el-icon-caret-right"/></i> 내가 생각한 해결 방안
                <span>
                <ol>
                  <li style = 'padding : 10px 0 10px 0'>
                    차장님 database 를 두 개로 관리하면 안될까요 ? 
                      <ol>
                        <li  style = 'padding : 10px 0 10px 0'>
                          응 ,, 수빈아 운영이랑 개발을 구분하려고 데이터베이스 두 개 만드는건 좀 그러네 ..
                        </li>
                      </ol>
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    모든 테이블을 <span class='one'>개발 테이블</span>과 <span class='one'>운영 테이블</span>로 구분하자.
                    <ol>
                        <li  style = 'padding : 10px 0 10px 0'>
                          운영 테이블은 유지하였습니다.
                        </li>
                        <li  style = 'padding : 5px 0 10px 0'>
                          <span class='gubul' style = 'line-height : 50px'>개발 테이블은 접두어로 'DEVEL_{TABLE NAME}' 을 명시</span>해주었습니다. <br> (사실 참조중인 모든 테이블을 개발 테이블 생성하고 모든 mybatis 를 변경한다는게 쉽지 않았습니다.. 하지만 해놓으니까 이제는 모두가 편해요 !! )
                        </li>
                      </ol>
                  </li>
                  <li style = 'padding : 10px 0 10px 0'>
                    로딩시 제일 처음 IP 를 확인했습니다.
                    <ol>
                        <li  style = 'padding : 10px 0 10px 0'>
                          <span class='yellowfont'>운영서버 IP 가 아니라면</span> 전역변수를 사용하여 <span class='yellowfont'>모든 테이블명 앞에 'DEVEL_' 을 명시</span>해주었습니다. 
                        </li>
                    </ol>
                  </li>
                </ol>
                <span>
                  <i class="el-icon-caret-right"/></i> 해피엔딩 <br> &nbsp &nbsp 저희팀은 개발 / 운영 웹서버 반영시 분기에 대한 고민을 하지않고 반영후 충분한 테스트를 할 수 있었습니다.<br> <br> 
                <span>
              </div>
            </div>
            `
          }else if(Number(value) === 11){
            this.skillMsg =  
            `
            <div style = 'padding : 0 0 0 0px'>
              <span style = 'font-size:30px;'> 운영중이던 하나의 프로젝트에서 API 와 Front 의 도메인을 분리시키세요 ! </span><br><hr/><br>
              <div style = 'display: flex; justify-content: left; padding : 0 0 0 0'>
                <span>
                  Spring Boot + VueJs 로 하나의 프로젝트를 진행중이었는데 
                  <br><br>
                <span>
                <div style = 'height : 150px; width : 800px;'>
                  <div style = 'border :1px solid grey; height : 30px; width : 97.4%; padding : 10px; float : left; text-align : center'>
                      https://soobindeveloper8.binsoo.com
                  </div>
                  <div style = 'border :1px solid grey; height : 60px; width : 49.8%; float : left; text-align : center; padding : 38px 0 0 0'>
                    Spring boot
                  </div>
                  <div style = 'border :1px solid grey; height : 60px; width : 49.7%; float : left; text-align : center; padding : 38px 0 0 0'>
                   Vue Js
                  </div>
                </div> 
                <span>
                  <br> 두개의 도메인으로 분리해서 관리하자는 요구를 받았다
                  <br><br>
                <span>
                <div style = 'height : 150px; width : 800px;'>
                  <div style = 'border :1px solid grey; height : 30px; width : 47.4%; padding : 10px; float : left; text-align : center'>
                      https://soobindeveloper8<span style = 'color : red'>api</span>.binsoo.com
                  </div>
                  <div style = 'border :1px solid grey; height : 30px; width : 47%; padding : 10px; float : left; text-align : center'>
                      https://soobindeveloper8.binsoo.com
                  </div>
                  <div style = 'border :1px solid grey; height : 60px; width : 49.8%; float : left; text-align : center; padding : 38px 0 0 0'>
                    Spring boot
                  </div>
                  <div style = 'border :1px solid grey; height : 60px; width : 49.7%; float : left; text-align : center; padding : 38px 0 0 0'>
                   Vue Js
                  </div>
                </div> 
                <span>
                  <br> 이때 발생할 수 있는 상황이 cros 인데 <span class = 'gubul'>Origin 을 설정해줌으로써 해결</span>한 적이 있습니다.
                  <br><br>
                <span>
                <div style = 'height : 150px; width : 800px;'>
                  <div style = 'border :1px solid grey; height : 30px; width : 47.4%; padding : 10px; float : left; text-align : center'>
                      https://soobindeveloper8api.binsoo.com
                  </div>
                  <div style = 'border :1px solid grey; height : 30px; width : 47%; padding : 10px; float : left; text-align : center'>
                      https://soobindeveloper8.binsoo.com
                  </div>
                  <div style = 'border :1px solid grey; height : 60px; width : 49.8%; float : left; text-align : center; padding : 23px 0 15px 0'>
                    Access Control Allow Origin : <br> https://soobindeveloper8.binsoo.com
                  </div>
                  <div style = 'border :1px solid grey; height : 60px; width : 49.7%; float : left; text-align : center; padding : 23px 0 15px 0'>
                    Origin : <br>https://soobindeveloper8.binsoo.com
                  </div>
                </div> 
            </div>
            `
          }
        }// 
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
          alert('s')
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

.gitatag {
  color: black;
}


.gitatag:hover {
  color: white;
  background-color: green;
}

.vue-back {
  background-image: url("../../assets/lang/vue.jpg");
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