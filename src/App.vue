<template>
  <div id="app">
    <div style = "height: 100px; width: 100%; padding : 10px 0 0 0; margin : 0 0 30px 0; background : #06113C; color : white">
      <h1>백엔드 개발자 정수빈</h1>
    </div>
    <BinsooStep/>
  </div>
</template>

<script>
import BinsooStep from './components/step/BinsooStep.vue'

export default {
  name: 'App',
  components: {
    BinsooStep
  }

  , data() {
        return {
           
        }
      }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
