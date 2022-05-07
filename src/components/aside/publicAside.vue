<template>

  <div>
    <!--logo-->
    <div align="center">
      <div style="margin-top: 25%">
        <img :src="logoImgUrl" width="160" height="80">
      </div>

      <br/>

      <!--头像-->
      <div style="width: 80px; height: 80px; border-radius:40px; overflow: hidden; margin-top: 20%" @click="profileClick">
        <img :src="circleUrl" title="登录" style="width: 80px;height: 80px;">
      </div>

    </div>
  </div>


</template>

<script>
export default {
  name: "publicAside",
  data() {
    return {
      logoImgUrl: "../src/assets/img/yuuki.png",
      circleUrl: "../src/assets/img/login.png"
    }
  },
  methods: {
    profileClick() {
      if (this.circleUrl ===  "../src/assets/img/login.png") {
        this.login()
      }
    },
    login() {
      this.$router.push({path: "/login"})
    },
  }
}
</script>

<style scoped>
.block {
  margin-top: 20px;
  margin-left: 20px;
}
</style>
