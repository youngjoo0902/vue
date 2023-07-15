<template>
    <div id="gnb">
      <ul>
        <li class="list1" :class="idx == '1' ? ' on' : '' "><a href="#" @click="h(1)">메뉴1</a></li>
        <li class="list2" :class="idx == '2' ? ' on' : '' "><a href="#" @click="h(2)">메뉴2</a></li>
        <li class="list3" :class="idx == '3' ? ' on' : '' "><a href="#" @click="h(3)">메뉴3</a></li>
      </ul>
    </div>
</template>

<script>
export default {
  name : 'GnbMenu',
  data(){
      return {
        idx : 1
      }
    },
  methods : {
      h(i){
        console.log(this.idx);
        this.idx = i;
      }
    }
}
</script>

<style>

</style>