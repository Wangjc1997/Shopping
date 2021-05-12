<template>
  <header-top :title="title" />
</template>

<script>
import HeaderTop from "../../components/HeaderTop/HeaderTop.vue";
export default {
  components: { HeaderTop },
  data() {
    return {
      title: "订单列表",
    };
  },
  watch: {},
  created() {},
  mounted() {},
  methods: {},
};
</script>

<style>
</style>
