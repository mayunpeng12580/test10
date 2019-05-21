<template>
  <div class="product_nav">
    <div class="product_top">
      <img src="@/assets/product_img/1-1.png">
    </div>
    <div class="clear product_center">
      <ul class="left" v-for="(item,index) in nav" :key="index">
        <li>
          <img :src="item.img">
        </li>
        <li v-text="item.title"></li>
        <li class="clear">
          <span v-text="item.stp" class="product_nav_left"></span>
          <span v-text="item.stm" class="product_nav_right"></span>
        </li>
      </ul>
    </div>
  </div>
</template>

 
<script>
export default {
  data: function() {
    return {
      nav: [
        {
          title: "3T OCULAX 眼周穴位贴 护眼贴 缓解眼部疲劳 医疗级别产品 5片装",
          img: require("@/assets/product_img/2-1.jpg"),
          stp: "￥88",
          stm: "找相似"
        },
        {
          title: "3T OCULAX 眼周穴位贴 护眼贴 缓解眼部疲劳 医疗级别产品 5片装",
          img: require("@/assets/product_img/2-2.jpg"),
          stp: "￥99",
          stm: "找相似"
        },
        {
          title: "3T OCULAX 眼周穴位贴 护眼贴 缓解眼部疲劳 医疗级别产品 5片装",
          img: require("@/assets/product_img/2-2.jpg"),
          stp: "￥99",
          stm: "找相似"
        },
        {
          title: "3T OCULAX 眼周穴位贴 护眼贴 缓解眼部疲劳 医疗级别产品 5片装",
          img: require("@/assets/product_img/2-1.jpg"),
          stp: "￥88",
          stm: "找相似"
        },
        {
          title: "3T OCULAX 眼周穴位贴 护眼贴 缓解眼部疲劳 医疗级别产品 5片装",
          img: require("@/assets/product_img/2-1.jpg"),
          stp: "￥88",
          stm: "找相似"
        },
        {
          title: "3T OCULAX 眼周穴位贴 护眼贴 缓解眼部疲劳 医疗级别产品 5片装",
          img: require("@/assets/product_img/2-2.jpg"),
          stp: "￥99",
          stm: "找相似"
        },
        {
          title: "3T OCULAX 眼周穴位贴 护眼贴 缓解眼部疲劳 医疗级别产品 5片装",
          img: require("@/assets/product_img/2-2.jpg"),
          stp: "￥88",
          stm: "找相似"
        }
      ]
    }
  }
};
</script>


<style lang="less">
.product_nav {
  width: 100%;
  background-color: white;


  .product_top {
    width: 100%;
    height: 0.80rem;
    margin: 0.10rem 0 0 0;

    img {
      width: 100%;
    }
  }

  .product_center {
    width: 100%;

    ul {

      width: 50%;
      text-align: center;
      li:nth-child(1) {
        width: 96%;
        margin: 0 2%;
        img {
          width: 100%;
        }
      }

      li:nth-child(2) {
        width: 100%;
        height: 0.7rem;
        overflow: hidden;
        text-overflow: ellipsis;
        font-size: 0.26rem;
        color: #232326;
        line-height: 0.32rem; 
        padding: 0.1rem;
        box-sizing: border-box
      }

     li:nth-child(3){
         padding:0 0.2rem;
        box-sizing: border-box;margin-top: 0.1rem
     }

      li:nth-child(3) .product_nav_left {
        font-size: 0.32rem;
        color: #f23030;
        display: block;
        float: left;
      }

      li:nth-child(3) .product_nav_right {
        display: block;
        width: 1rem;
        height: 0.35rem;
        float: right;
        font-size: 0.22rem;
        color: #666;
        border: 1px solid #bfbfbf;
       
        text-align: center;
        line-height: 0.35rem;
        
      }
    }

    
  }
}
</style>
