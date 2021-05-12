<template>
  <div class="profile">
    <header-top :title="title"></header-top>
    <section>
      <router-link to="/login">登录注册</router-link>
    </section>
  </div>
</template>

<script>
import HeaderTop from "../../components/HeaderTop/HeaderTop.vue";
export default {
  components: { HeaderTop },
  data() {
    return {
      title: "我的",
    };
  },
  watch: {},
  created() {},
  mounted() {},
  methods: {},
};
</script>

<style>
.profile {
  width: 100%;
  overflow: hidden;
}
</style>
