<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>Q0 : App.vue 파일명은 왜 빨간색이고, App.vue 소스에 <span class="code">&lt;HelloWorld /&gt;</span> 에 빨간 밑줄이 그어져 있나?</p>
    <p>Q1 : HeaderPage.vue에 보면, <span class="code">import GnbMenu from './views/layout/NavigationPage.vue'</span> 경로로 치면 에러 뜬다. <span class="code">'@/views/layout/NavigationPage'</span> 이거랑 <span class="code">./Navigation.vue</span> 는 잘된다. 이유가 뭐고, 에러는 어떻게 보는가?</p>
    <p>Q2 : 회사에서 views 폴더는 화면용인거 같아서, components 폴더를 만들어서 컴포넌트 불러왔는데 에러가 뜬다... 뭔가 설정이 필요하나? 여기서는 잘되네...</p>
    <p>Q3 : 헤더 영역에 버튼 클릭시 #app 에 클래스 토글</p>
    <p>Q4 : Gnb에서 클릭한 메뉴 addClass on, siblings removeClass on</p>
    <p>Q5 : 소스를 열 수 없는 상황에서, 개발자 도구만으로 디버깅 방법?</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
