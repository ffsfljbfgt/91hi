<template>
  <section class="container">
	<div class="tab-home tab-nav">
		<h2 class="tab-item fl active i-nav" data-id="1">海淘推荐</h2>
		<h2 class="tab-item fl i-nav" data-id="2">海淘优惠</h2>
		<h2 class="tab-item fl i-nav" data-id="3">海淘攻略</h2>
	</div>
</section>
</header>
  </div>
</template>

<script>
export default {

}
</script>


<style lang="scss" >
.tab-home {
    height: 60px;
    border-bottom: 1px solid #cfcfcf;
    width: 100%;
    position: fixed;
    top: 50px;
    z-index: 9999;
    background-color: #fff;
    max-width: 640px;
}
.tab-home .tab-item.active {
    border-bottom: 10px solid #ed7878;
    height: 51px;
}
.tab-home .tab-item {
    height: 60px;
    width: 33.3%;
    text-align: center;
    line-height: 60px;
    color: #3a3a3a;
    font-size: 18px;
}
</style>

