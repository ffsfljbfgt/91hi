<template>
    <div>
        <div class="login-top">
            <a class="login-back" href="javascript:history.back();"><img src="http://m.91lai.com/assets/Home/images/btn-close.png"></a>
        <div class="login-title">手机快捷登录</div>
        <div class="detail login-box" style="margin: 0 20px;">
            <form id="loginform" name="login" method="post" action="http://m.91lai.com/index.php/Login/mobilelogin">
            <div class="login-cons" style="margin-left:-2px;">
            <div class="form-item">
            <div class="user_login_input_mobile form-item">
            <input type="text" name="mobile" id="mobile" placeholder="请输入手机号">
            <button type="button" disabled="true" class="btn-captcha" id="login_mobile_code">获取验证码</button>
        </div>
            <span id="tips_mobile"></span>
            </div>
            <div class="form-item">
                <div class="user_login_input_mobile">
                    <input type="text" name="checkcode" id="checkcode" placeholder="请输入验证码" style="width:98%;">
                </div>
            </div>
            <div class="m-login">
                <a href="http://m.91lai.com/index.php/login.html" class="account">账号密码登录</a>
                <a href="http://m.91lai.com/index.php/Register" class="reg">注册</a>
            </div>
            <input type="submit" id="logintj" disabled="true" class="btn_login" value="登录" title="登录">

            </div>
            </form>
        </div>
    </div>
    <div class="detail login-box" style="margin: 0 20px;">
    <form id="loginform" name="login" method="post" action="http://m.91lai.com/index.php/Login/mobilelogin">
        <div class="login-cons" style="margin-left:-2px;">
            <div class="form-item">
                <div class="user_login_input_mobile form-item">
                    <input type="text" name="mobile" id="mobile" placeholder="请输入手机号">
                    <button type="button" disabled="true" class="btn-captcha" id="login_mobile_code">获取验证码</button>
                </div>
                <span id="tips_mobile"></span>
            </div>
            <div class="form-item">
                <div class="user_login_input_mobile">
                    <input type="text" name="checkcode" id="checkcode" placeholder="请输入验证码" style="width:98%;">
                </div>
            </div>
            <div class="m-login">
                <a href="http://m.91lai.com/index.php/login.html" class="account">账号密码登录</a>
                <a href="http://m.91lai.com/index.php/Register" class="reg">注册</a>
            </div>
            <input type="submit" id="logintj" disabled="true" class="btn_login" value="登录" title="登录">

        </div>
    </form>
</div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scope>
    .login-top {
    width: 100%;
    color: #fff;
    height: 200px;
    overflow: hidden;
    margin-top: -88px;
    background: #f15757;
}
.login-back {
    float: left;
    margin-top: 50px;
    margin-left: 50px;
}
img {
    border: 0;
}
.login-title {
    margin-top: 120px;
    margin-left: 50px;
    font-size: 20px;
}
form {
    display: block;
    margin-top: 0em;
}
.form-item {
    margin: 15px 0;
}
.user_login_input_mobile input {
    border: none;
    border-bottom: 1px solid #d4d4d4;
    height: 50px;
    width: 50%;
    padding-left: 10px;
    font-size: 16px;
}
button[disabled], html input[disabled] {
    cursor: default;
}
.btn-captcha {
    display: inline-block;
    float: right;
    width: 36%;
    height: 50px;
    font-size: 16px;
    color: #fff;
    background: #808080;
    border: none;
    border-radius: 5px;
}
.user_login_input_mobile input {
    border: none;
    border-bottom: 1px solid #d4d4d4;
    height: 50px;
    width: 50%;
    padding-left: 10px;
    font-size: 16px;
}
.m-login {
    margin-top: 80px;
}
.m-login a {
    color: #FB4B4B;
    font-size: 16px;
    display: inline-block;
    width: 48%;
}
.m-login .reg {
    text-align: right;
}
.btn_login {
    width: 90%;
    height: 40px;
    color: #fff;
    font-size: 16px;
    background: #808080;
    position: fixed;
    bottom: 0;
    border: none;
    border-radius: 5px;
    right: 18px;
}
</style>