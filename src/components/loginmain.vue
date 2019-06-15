<template>
    <div id="bibox">
        <div class="divider"></div>
        <div class="tab-content-home detail" style="margin-top: 1em;">
		<form id="loginform" name="login" >
		    <input type="hidden" name="ecmsfrom" value="">
		   <ul>
			    <li class="user_login_not_fli">
			       <div class="user_login_input_wrap">
				       <div class="user_login_icon_head"></div>
				       <input type="text" id="username" placeholder="请输入用户名">
			       </div>
			    </li>
			    
			    <li class="user_login_not_fli">
			    	<div class="user_login_input_wrap">
			    	    <div class="user_login_icon_ps"></div>
			        	<input type="password" id="password" placeholder="请输入密码">
			        </div>
			     </li>
			    
			   <li> 
				    <div class="login_bt_comfirm">
				      <input type="button" id="logintj" value="登录" title="登录" v-on:click="Login">
				    </div>
			    </li>
			    
			    <li>
			    	<a href="/reg" class="login_link_2re">
                				<span class="gold1">立即注册</span>
            			</a>
				<a href="" class="login_link_2re" style="float:right;">
                				<span class="gold1">找回密码</span>
            			</a>
			    </li>
		    </ul>
		  </form>
	</div>
    </div>
</template>
<script>
import axios from "axios"
export default {
     data(){
        return{
            usname:"",
            pword:""
        }
    },
    methods: {
    Login:function(){
        this.usname = document.querySelector("#username").value
        this.pword = document.getElementById("password").value
        this.getMainInfo()
    },
    getMainInfo:function(){
    axios.get("http://localhost:3000/sf/ad?"+"u="+this.usname+"&p="+this.pword)
    .then(this.getMainInfoSucc)},
    
	getMainInfoSucc:function(res){
		 if(res.data[0]){
             if(res.data[0].pword==this.pword){
                 alert("登陆成功")
             }else{
                 alert("登陆失败")
             }
         }else{
             alert("登陆失败")
         }
     },
   

     
  },
}
</script>
<style  scope>
.divider {
    height: 10px;
    background-color: #f5f5f5;
    margin: 0 auto;
}
form {
    display: block;
    margin-top: 0em;
}
button, input, optgroup, select, textarea {
    color: inherit;
    font: inherit;
    margin: 0;
}
.user_login_not_fli {
    clear: both;
    float: none;
    margin-top: 1.5em;
    padding: 0 10px;
}
.user_login_input_wrap {
    height: 3.8em;
    width: 100%;
    background: #f7f7f8;
    border: 1px solid #d4d4d4;
    position: relative;
}
.user_login_input_wrap div, .user_login_input_wrap input {
    vertical-align: middle;
    overflow: hidden;
    word-break: keep-all;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    display: inline-block;
}
.user_login_icon_head {
    float: left;
    width: 3.8em;
    height: 3.8em;
    background: url(../images/reg.png) -1.5em -6em no-repeat;
    background-size: 30em 25em;
}
.user_login_input_wrap input {
    background: none;
    border: none;
    height: 96%;
    font-size: 16px;
    color: #949292;
    text-indent: 1em;
    width: 74%;
}
.user_login_input_wrap div, .user_login_input_wrap input {
    vertical-align: middle;
    overflow: hidden;
    word-break: keep-all;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    display: inline-block;
}
.login_bt_comfirm {
    margin: 20px auto;
    width: 96%;
    height: 50px;
    display: block;
    background: #F15757;
}
.login_bt_comfirm input {
    width: 100%;
    height: 100%;
    border: none;
    text-align: center;
    font-size: 16px;
    color: #fff;
    background: none;
}
.user_login_input_wrap .user_login_icon_ps {
    float: left;
    width: 3.8em;
    height: 3.8em;
    background: url(../images/reg.png) -7em -6em no-repeat;
    background-size: 30em 25em;
}
.login_link_2re {
    width: 50%;
    height: 40px;
    line-height: 40px;
    display: block;
    text-align: center;
    float: left;
    text-decoration: none;
    color: red
}
.login_link_2re {
    width: 50%;
    height: 40px;
    line-height: 40px;
    display: block;
    text-align: center;
    float: right;
    text-decoration: none;
     color: red
}
#bibox{
    margin-top: 3.4rem;
}

</style>