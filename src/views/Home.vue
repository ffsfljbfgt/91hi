<template>
  <div class="home">
    <HomeHeader/>
    <Homenav/>
    <Homemain/>
    <homefooter/>
  </div>
</template>

<script >
import HomeHeader from './HomeHeader.vue'
import Homenav from '../components/Homenav.vue'
import Homemain from '../components/Homemain.vue'
import homefooter from "../components/homefooter.vue"
export default {
   components:{
      HomeHeader,
      Homenav,
      Homemain,
      homefooter
  }
}
</script>


<style lang="scss" >

</style>

