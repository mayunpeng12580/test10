<template>
	
	<div id="product">
		<top-bar>
			
			<div class="nav-tab">
				
				<ul class="flex">
					<li class="flex-item" :class="{active:index==navIndex}" v-for="(item,index) in nav" @click="navIndex=index;" >
						<span v-text="item.title"></span>
					</li>
				</ul>
				
			</div>
			
		</top-bar>
		
		<h1>{{ $route.params.id  }}</h1>
		
		<h1> 
		
		  <a href="/">首页</a>
		
		</h1>
		
	</div>
	
</template>

<script>
	
	import TopBar from "@/components/TopBar";
	
	
	export default{
		data(){
			return {
				navIndex:0,
				nav:[{title:'商品'},{title:'评价'},{title:'详情'},{title:'推荐'}]
			};
		},
		components:{
			TopBar
		},
		created(){
			// 全局路由对象
			console.log(this.$router);
			// 当前页面的路由对象
			console.log(this.$route);
			
//			console.log(this.$route.params.id);
		}
	}
	
	
</script>

<style lang="less">
	
	.nav-tab{
		padding: 0 0.6rem;
		line-height: 0.9rem;
		text-align: center;
		
		li.active span{
			color:  #e4393c;
			padding-left: 0.26rem;
			background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAYBAMAAAABjmA/AAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAAAnUExURek7PUdwTO49Peg6Peo6Puc6Pek6POk6POg6POg7PeY8POg6POk6PApBjXgAAAANdFJOU/8ADttQPYvEqJYqW/KuifCQAAAAjklEQVQI10XOsRGCQBAF0D8eA6Imn4ERMh0tgDE2UDqgA2Ij7UA6gA6MjCnB0vzLBlxw92Z379+B/F7DgwQraI3C05AQc0ElfBCac40NOlzIE2LUuJM5gtpHMtPxc+yW1tuH15j8+hYHD1yhdPQoHO3yKG+GSNgbXsI81AocgNS+qlgLFwrrGNjFdFS9tj82HhIeoIR1QQAAAABJRU5ErkJggg==);;
			background-size: 0.16rem;
			background-repeat: no-repeat;
			background-position: left center;
		}
	}
	
</style>