<template>
    <div>
       <LoginHeader/> 
       <LoginMain/> 
       <LoginFooter/> 
    </div>
</template>
<script>
import LoginHeader from './HomeHeader.vue'
import LoginFooter from '../components/homefooter.vue'
import LoginMain from '../components/loginmain.vue'

export default {
 
    components:{
        LoginHeader,
        LoginFooter,
        LoginMain
    },
 
}
</script>
<style lang="scss" scope>
    
</style>