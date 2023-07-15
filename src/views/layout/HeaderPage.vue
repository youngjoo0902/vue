<template>
  <div id="header">
    <p>헤더</p>
    <button @click="func">클릭하면 #app 에 on 클래스가 토글되야 함</button>
    <GnbMenu />
  </div>
</template>

<script>
  import GnbMenu from '@/views/layout/NavigationPage'

export default {
    name : 'HeaderPage',
    props : {
      isHeaderOpened : Boolean
    },
    data(){
      return {
        func(){
          //여기서 부모 데이터에 쓰기가 안되나?
          if(this.isHeaderOpened != true){
            console.log(1);
            //this.isHeaderOpened = true;
          }else{
            console.log(2);
            //this.isHeaderOpened = false;
          }
        }
      }
    },
    components: {
      GnbMenu
    }
}
</script>

<style>
</style>