<template>
  <div class="home">
  	<search-bar></search-bar>
  	<swiper></swiper>
  	<quick-nav></quick-nav>
	<product-nav></product-nav>
	<nav-bar></nav-bar>
  </div>
</template>

<script>

import SearchBar from "@/components/SearchBar";
import Swiper from "@/components/HomeSwiper";
import QuickNav from "@/components/QuickNav";
import NavBar from "@/components/NavBar";
import ProductNav from "@/components/ProductNav";

export default {
  name: 'home',
  components: {
  	SearchBar,
  	Swiper,
  	QuickNav,
  	NavBar,
	ProductNav
  }
}
</script>

<style >
	
	
</style>