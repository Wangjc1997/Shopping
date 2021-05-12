<template>
  <div class="login">
    <div @click="$router.back()">返回</div>
    <section class="account">
      <input type="text" />
    </section>
    <section class="password">
      <input type="password" />
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style>
.login {
  display: flex;
  flex-direction: column;
}
.account {
  font-size: 16px;
}
</style>
