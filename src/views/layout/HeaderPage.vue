<template>
  <div class id="header">
    <p>헤더</p>
    <button @click="headderToggle">클릭하면 #app 에 on 클래스가 토글되야 함</button>
    <GnbMenu />
  </div>
</template>

<script>
  import GnbMenu from '@/views/layout/NavigationPage'

export default {
    name : 'HeaderPage',
    data(){
      return {
        isToggle : ''
      }
    },
    components: {
      GnbMenu
    },
    methods : {
      headderToggle(){
        this.$emit('headerEmit', this.isToggle)
      }
    }
}
</script>

<style>
</style>