<template>
  <div id="app">
    <div style = "height: 100px; width: 100%; padding : 30px 0 0 0; margin : 0 0 0 0; background : white; display: flex; justify-content: left;">
      <div style="width: 70%; text-align : right; float: left;">
        <h1 style = "font-color : black; font-family: BMHANNA_11;"> 느려도 꾸준히 나아가는, 백엔드 개발자 정수빈 입니다.</h1>
      </div>
      <div style="width: 30%; padding : 0 30px 0 0; float: left; font-family: BMEULJIROTTF;">
        <div style="height: 30px; width: 100%; text-align: right; font-size : 25px; margin : 0 0 20px 0 ; cursor: pointer;" @click="windowOpen('https://soobindeveloper8.tistory.com')" @mouseover="blogStatus = false" @mouseout="blogStatus = true">
            <div v-if="blogStatus" style="height: 30px; width: 100%; text-align: right">블로그 가기</div>
            <div v-else style="height: 30px; width: 100%; text-align: right">제 다이어리같은 개발 기록들이에요 !</div>
        </div>
        <div style="height: 30px; width: 100%; text-align: right; font-size : 25px; cursor: pointer;" @click="windowOpen('https://github.com/soobinJung')" @mouseover="gitStatus = false" @mouseout="gitStatus = true">
            <div v-if="gitStatus" style="height: 30px; width: 100%; text-align: right">깃 가기</div>
            <div v-else style="height: 30px; width: 100%; text-align: right">잔디가 노력의 증표는 아니잖아요 .. <br> ( 참고 : 쉬엄쉬엄 성장 한 적 없음 !! )</div>
        </div>
      </div>
    </div>
    <BinsooStep style="margin : 0 0 50px 0"/>
    <BinsooSkill style="width: 100%; height: 900px;" />
    <BinsooSide style="margin : 50px 0 100px 0"/>
    <BinsooStudy/>
    <BinsooBook/>
  </div>
</template>

         
<script>
import BinsooStep from './components/step/BinsooStep.vue'
import BinsooSkill from './components/skill/BinsooSkill.vue'
import BinsooBook from './components/books/BinsooBook.vue'
import BinsooStudy from './components/study/BinsooStudy.vue'
import BinsooSide from './components/side/BinsooSide.vue'
import BMHANNAPro from './assets/font/BMHANNAPro.ttf'

export default {
  name: 'App',
  components: {
    BinsooStep
    , BinsooSkill
    , BinsooBook
    , BinsooStudy
    , BinsooSide
    , BMHANNAPro
  }

  , data() {
    return {
        blogStatus : true
        , gitStatus : true
    }
  }

  , methods : {
    windowOpen(url){
      window.open(url)
    }
  }
}
</script>

<style>

@font-face { /* 애플산돌고딕 폰트 적용 */
  font-family: "BMHANNAPro";
  src: url("./assets/font/BMHANNAPro.ttf") format("truetype");
  font-weight: normal;
} 

@font-face { /* 애플산돌고딕 폰트 적용 */
  font-family: "BMHANNA_11";
  src: url("./assets/font/BMHANNA_11yrs_ttf.ttf") format("truetype");
  font-weight: normal;
} 

@font-face { /* 애플산돌고딕 폰트 적용 */
  font-family: "BMEULJIROTTF";
  src: url("./assets/font/BMEULJIROTTF.ttf") format("truetype");
  font-weight: normal;
} 


@font-face { /* 애플산돌고딕 폰트 적용 */
  font-family: "BMYEONSUNG";
  src: url("./assets/font/BMYEONSUNG_ttf.ttf") format("truetype");
  font-weight: normal;
} 


.gubul{
  text-decoration-style : wavy;   text-decoration-line: underline; text-decoration-color: red;  text-underline-position: under;
 
}

.one{
  border-radius: 50%; border : 2px solid red
}
/* #app {
  font-family: BMHANNAPro;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
} */
</style>
