<template>
<div>
  <HeaderPage @headerEmit="headerEmitToggle" />

  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="css는 대충 만들어놨음" />
  </div>
</template>

<script>
import './assets/css/common.css'

import HelloWorld from './components/HelloWorld'
import HeaderPage from './views/layout/HeaderPage'

export default {
  name: 'App',
  components: {
    HeaderPage,
    HelloWorld
  },
  data(){
    return {
    }
  },
  methods : {
    headerEmitToggle(){
      console.log(111);
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
