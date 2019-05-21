<template>
	
	<div>
		
		<div class="box"></div>
		<h1>购物车</h1>
		
		<product-nav></product-nav>
		
		<nav-bar></nav-bar>
	</div>
	
</template>

<script>
	import NavBar from "@/components/NavBar";
	import ProductNav from "@/components/ProductNav";
	
	export default{
		components:{
			NavBar,
			ProductNav
		}
	}
	
</script>

<style>
</style>