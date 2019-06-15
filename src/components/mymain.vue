<template>
    <div>
        <div class="tab-content-user detail">
    <div class="md_content">
        <div class="my_top">

            <div class="u_intro_login">
                <img src="http://m.91lai.com/assets/Home/images/head.png" height="100" width="100">
            </div>
            <div class="jifen">
                <div class="u_login" style="margin-top: 20px;">
                    <a href="./login" class="u_s">尚未登录</a>
                    <a href="" class="lbn"></a>
                </div>
                <ul class="u_profile">
                    <li>
                        <p>0</p>
                        <p>等级</p>
                    </li>
                    <li>
                        <p>0</p>
                        <p>积分</p>
                    </li>
                    <li>
                        <p>0</p>
                        <p>金币</p>
                    </li>
                </ul>
            </div>
        </div>


        <div class="apply">
            <ul>

                <li>
		    <a href="http://m.91lai.com/rebate/info">
			    			<span><img alt="" src="http://m.91lai.com/assets/Home/images/us1.png"></span>
			    			<span>返利中心</span>
		    </a>
	       </li>
		    		
		    		<li>
		    			<a href="http://m.91lai.com/rebate/index">
			    			<span><img alt="" src="http://m.91lai.com/assets/Home/images/us2.png"></span>
			    			<span>订单管理</span>
		    			</a>
		    		</li>
		    		
		    		
		    		<li>
		    			<a href="http://m.91lai.com/rebate/mingxi">
			    			<span><img alt="" src="http://m.91lai.com/assets/Home/images/us3.png"></span>
			    			<span>账目明细</span>
		    			</a>
		    		</li>
		    		
		    		
		    		<li>
		    			<a href="http://m.91lai.com/index.php/user/favorite">
			    			<span><img alt="" src="http://m.91lai.com/assets/Home/images/us4.png"></span>
			    			<span>我的收藏</span>
		    			</a>
		    		</li>
		    		
		    		<li>
		    			<a href="http://m.91lai.com/handbook/jfdh/">
		    				<span><img alt="" src="http://m.91lai.com/assets/Home/images/us5.png"></span>
		    				<span>豪礼兑换</span>
		    			</a>
		    		</li>
		    		
		    		<li>
		    			<a href="http://m.91lai.com/index.php/user/comment">
		    				<span><img alt="" src="http://m.91lai.com/assets/Home/images/us6.png"></span>
		    				<span>评论留言</span>
		    			</a>
		    		</li>
		    		
		    		<li>
		    			<a href="http://m.91lai.com/index.php/user/baoliao">
		    				<span><img alt="" src="http://m.91lai.com/assets/Home/images/us7.png"></span>
		    				<span>我的爆料</span>
		    			</a>
		    		</li>
		    		
		    		<li>
		    			<a href="http://m.91lai.com/index.php/user/profile">
		    				<span><img alt="" src="http://m.91lai.com/assets/Home/images/us8.png"></span>
		    				<span>个人信息</span>
		    			</a>
		    		</li>

            </ul>
        </div>
       
    </div>
</div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
    .tab-content-user {
    background: #F6F5FB;
    overflow: hidden;
}
.my_top {
    background: url(../images/mymain.png) no-repeat center;
}
.u_intro_login {
    overflow: hidden;
    text-align: center;
    padding-top: 64px;
}
.u_intro_login img {
    border-radius: 60px;
}
.jifen {
    text-align: center;
    overflow: hidden;
    padding-bottom: 40px;
}
.u_login {
    font-size: 18px;
    color: #fff;
}
.u_s {
    color: #fff;
    padding-left: 40px;
}
.u_login {
    font-size: 18px;
    color: #fff;
}
.u_profile {
    margin-top: 0;
    overflow: hidden;
    -webkit-padding-start: 0px;
}
.u_profile li {
    float: left;
    width: 33.3%;
}
.u_profile li p:nth-child(1) {
    font-size: 16px;
}
.u_profile li p {
    color: #fff;
}
p {
    display: block;
    margin-block-start: 1em;
    margin-block-end: 1em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
}
.u_profile li {
    float: left;
    width: 33.3%;
}
.u_profile li p:nth-child(2) {
    font-size: 12px;
}
.u_intro_login img {
    border-radius: 60px;
}  
.u_intro_login {
    overflow: hidden;
    text-align: center;
    padding-top: 64px;
}
.lbn {
    background: url(../images/mymain1.png) no-repeat center;
    background-size: 20px;
    height: 20px;
    width: 20px;
    float: right;
    margin-top: 3px;
    margin-right: 20px;
}
.u_profile[data-v-e76c2616] {
  list-style: none;
}
.apply {
    background: #fff;
    overflow: hidden;
    padding-top: 30px;
}
.apply ul {
    overflow: hidden;
    padding-left: 0;
    width: 100%;
}
.apply ul li {
    float: left;
    width: 33.3%;
    margin-top: 10px;
    margin-bottom: 20px;
}
.apply ul li a {
    color: #101010;
}
ol, ul, li {
    list-style: none;
}
a {
    text-decoration: none;
}
.apply ul li span {
    display: block;
    text-align: center;
}
.apply ul li img {
    width: 62px;
    height: 62px;
}
.apply ul li span:nth-child(2) {
    text-align: center;
    font-size: 14px;
    color: #818181;
}
.apply ul li  {
  height: 85px;
}
.apply{
    height: 500px;
}
</style>
