<template>
    
    <footer class="container">
        <div class="bottom-nav" id="bottom-nav" v-on:click="FooterRouter">  
            <router-link to="/"  class="home b_1" id="home">首页</router-link>
            <a href="" class="category" id="category">分类</a>
            <a href="" class="broke" id="broke">爆料</a>
            <router-link to="/my"  class="my" id="my">我的</router-link>
	    </div>
    </footer> 
</template>
<script>
export default {
    methods: {
       
        getElement:function(){
            var home =document.getElementById("bottom-nav").children[0]
            var category =document.getElementById("bottom-nav").children[1]
            var broke =document.getElementById("bottom-nav").children[2]
            var my =document.getElementById("bottom-nav").children[3]
        },
        FooterRouter:function(e){
            this.getElement()
            if (e.target.id=="my") {
                this.MyChange()
            }
        },
        MyChange:function(){
            my.className="myr"
            home.className="homer"
            category.className="category"
            broke.className="broke"
        }
    },
    mounted() {
        if(window.location.href=="http://localhost:8080/my"){
              this.MyChange()
        }
        
    },
}
</script>
<style lang="scss" scope>
footer .bottom-nav {
    width: 100%;
    height: 77px;
    background-color: #fff;
    position: fixed;
    bottom: 0;
    z-index: 9999;
    border-top: 1px solid #EFEFEF;
    max-width: 640px;
}

footer .bottom-nav a {
    display: block;
    width: 25%;
    height: 77px;
    float: left;
    color: #383838;
    font-size: 16px;
    text-align: center;
    line-height: 110px;
    background-size: 30%;
}
footer .bottom-nav a.home {
    background: url(../images/footer1r.png) no-repeat center 15px;
    background-size: 30%;
}
footer .bottom-nav a.homer {
    background: url(../images/footer1.png) no-repeat center 15px;
    background-size: 30%;
}
footer .bottom-nav a.category {
    background: url(../images/footer2.png) no-repeat center 15px;
    background-size: 30%;
}
footer .bottom-nav a.broke {
    background: url(../images/footer3.png) no-repeat center 15px;
    background-size: 30%;
}
footer .bottom-nav a.my {
    background: url(../images/footer4.png) no-repeat center 15px;
    background-size: 30%;
}
footer .bottom-nav a.myr {
    background: url(../images/footer4r.png) no-repeat center 15px;
    background-size: 30%;
}
footer .bottom-nav a{
    text-decoration: none;  
}
</style>