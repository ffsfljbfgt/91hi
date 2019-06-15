<template>
  <div style="margin-top:2.9em">
    <div class="divider"></div>
    <div class="tab-content-home  detail" style="margin-top: 1em;">
		<form id="loginform" name="login" >
		    <input type="hidden" name="ecmsfrom" value="">
		    <ul>
			    <li class="user_login_not_fli">
			      <div class="user_login_input_wrap">
					<div class="user_login_icon_head"></div>
			      	<input type="text" id="membername" name="username" placeholder="请输入账号"  v-on:keyup="press" >
			      </div>
			    </li>
			    
			    <li class="user_login_not_fli">
			    	<div class="user_login_input_wrap">
				    	<div class="user_login_icon_ps"></div>
			      		<input type="password" id="memberpwd" name="password" placeholder="请输入密码" v-on:keyup="press">
			      	</div>
			    </li>
			   
			    <li class="user_login_not_fli">
			    	<div class="user_login_input_wrap">
			    		<div class="user_login_icon_cfps"></div>
			      		<input type="password" id="rpword" name="repassword" placeholder="再次输入密码" v-on:keyup="press">
			      	</div>
			    </li>
			   
			    
			    <li class="user_login_not_fli">
			    	<div class="user_login_input_wrap">
				    	<div class="user_login_icon_mess"></div>
				        <input type="text" id="email" name="email" placeholder="输入邮箱" v-on:keyup="press">
			        </div>
			    </li>
			    
			    
			    <li>
			    	<div class="login_bt_comfirm">
			      		<input type="button" id="logintj" value="立即注册" v-on:click="ackv">
			      	</div>
			    </li>
			    
		    </ul>
		  </form>
	</div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            uname:"",
            pword:"",
            emai:"",
            rpword:""
        }
    },
    methods: {

    // 插入账号密码
    RegUp:function(){
    axios.get("http://localhost:3000/sf/ad?"+"u="+this.usname+"&p="+this.pword)
    .then(this.getMainInfoSucc)}
    ,
	getMainInfoSucc:function(res){
     },
    press:function(){
        this.uname = document.getElementById("membername").value
        this.pword = document.getElementById("memberpwd").value
        this.emai = document.getElementById("email").value
        this.rpword = document.getElementById("rpword").value
        console.log(this.uname,this.pword,this.emai)
    },
    ackv:function(){
       if(this.pword==this.rpword){
           console.log(666)
       }
    }
    },
    mounted() {
        console.log(this.uname)
    },
}
</script>


<style lang="scss" scope>
  .divider {
    height: 10px;
    background-color: #f5f5f5;
    margin: 0 auto;
}
html{
    font-size: 18px;
}
form {
    display: block;
    margin-top: 0em;
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
.user_login_icon_head {
    width: 68px;
    height: 68px;
    background: url(../images/reg.png) -1.5em -6em no-repeat;
    background-size: 30em 25em;
    float: left;
}
.user_login_input_wrap .user_login_icon_ps {
    width: 3.8em;
    height: 3.8em;
    background: url(../images/reg.png) -7em -6em no-repeat;
    background-size: 30em 25em;
    float: left;
}
.user_login_input_wrap .user_login_icon_cfps {
    width: 3.8em;
    height: 3.8em;
    background: url(../images/reg.png) -18.5em -6em no-repeat;
    background-size: 30em 25em;
    float: left;
}
.user_login_input_wrap .user_login_icon_mess {
    width: 3.8em;
    height: 3.8em;
    background: url(../images/reg.png) -12.5em -6em no-repeat;
    background-size: 30em 25em;
    float: left;
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
</style>

