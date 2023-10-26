<template>
  <div class="container1">
    <main-header/>
      <router-view/>
    <main-footer/>
  </div>
</template>

<script>

import MainHeader from '@/components/includes/MainHeader.vue'
import MainFooter from './components/includes/MainFooter.vue';

  export default{
    name: 'App',
    components:{
    MainHeader,
    MainFooter
}
  }
</script>

<style lang="scss">
 *{
  padding: 0px;
  margin: 0px;
  
 }
 .container1{
  background: $color5;
 }
</style>
