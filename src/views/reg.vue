<template>
    <div>
        <RegHeader/>
        <regmain/>
        <Regfooter/>
    </div>
</template>
<script>
import RegHeader from './HomeHeader.vue'
import Regfooter from '../components/homefooter.vue'
import regmain from '../components/regmain.vue'
export default {
 components:{
     RegHeader,
     Regfooter,
     regmain
 }
    
}
</script>
<style lang="scss">
    
</style>