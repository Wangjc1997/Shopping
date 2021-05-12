<template>
  <div class="msite">
    <header-top :title="title">
      <span class="header_search" slot="left"
        ><i class="iconfont icon-sousuo"></i
      ></span>
      <span class="header_login" slot="right"
        ><span class="header_login_text">登录|注册</span></span
      >
    </header-top>
    <nav class="msite_nav">
      <div class="swiper-container">
        <div class="swiper-wrapper">
          <div class="swiper-slide">1</div>
          <div class="swiper-slide">2</div>
        </div>
        <!-- swiper轮播图圆点 -->
        <div class="swiper-pagination"></div>
      </div>
    </nav>
    <shop-list></shop-list>
  </div>
</template>

<script>
import swiper from "swiper";
import "swiper/swiper.min.css";

import HeaderTop from "../../components/HeaderTop/HeaderTop.vue";
import ShopList from "../../components/ShopList/ShopList.vue";

export default {
  mounted() {
    new swiper(".swiper-container", {
      loop: true,
      pagination: {
        el: ".swiper-pagination",
      },
    });
  },
  components: { HeaderTop, ShopList },
  data() {
    return { title: "哈哈哈哈" };
  },
};
</script>

<style>
.msite_nav {
  margin-top: 45px;
  height: 200px;
  background: #fff;
}
</style>
