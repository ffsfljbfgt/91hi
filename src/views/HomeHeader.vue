<template>
  <div >
  <header class="container">
	<div class="top-nav bgc-red">
		<a href="http://m.91lai.com/"><h1 class="logo fl" title="就要来海淘网"></h1></a>
		<div class="search-form fl">
			<form action="http://m.91lai.com/index.php/search" method="post">
				<input type="submit" class="smt" value="">
				<input type="text" name="keyword" class="text">
			</form>
		</div>
		<a class="notice fl dis-b" href="http://m.91lai.com/index.php/user/news">
					</a>
	</div>
   
</header>
  </div>
</template>

<script>
export default {

}
</script>


<style lang="scss" >

.fl {
    float: left;
}
header .top-nav {
    width: 100%;
    position: fixed;
    top: 0;
    z-index: 9999;
    max-width: 640px;
}
.bgc-red {
    background-color: #f15757;
}
a {
    text-decoration: none;
}
.logo {
    background:  url(../images/logo.png) no-repeat;
    width: 26%;
    height: 30px;
    margin: 10px 2%;
}
.search-form {
    background:  url(../images/search.png) no-repeat 6px center;
    width: 57%;
    height: 30px;
    border-radius: 3px;
    margin: 10px 0px 10px 0;
    background-color: #fff;
}
.search-form form {
    height: 30px;
}
.search-form .smt {
    width: 45px;
    padding: 0;
}
.search-form input {
    width: 100%;
    height: 30px;
    border: none;
    color: #757575;
    font-size: 15px;
    background: none;
    outline: none;
}
.search-form .text {
    width: 75%;
    position: relative;
    top: -10px;
    margin-left: -5px;
    height: 30px;
}
.notice {
    background:  url(../images/message.png)no-repeat center center;
    width: 9%;
    height: 30px;
    margin-top: 10px;
    position: relative;
    margin-left: 2%;
} 

</style>

