<template>
  <div class="Header">
    <img :src="jpg" class="jpg">
    <img :src="jiao" alt class="jiao" @click="Previous_page">
    <p class="zhu">{{registe}}</p>
    <div class="body">
      <hr class="hr1" color="#e6e6e6" size="0.01px">
      <p class="z1">{{MB}}</p>
      <input type="text" placeholder="请输入手机号" class="k1" style="outline:none;">
      <hr class="hr2" color="#e6e6e6" size="0.01px">
      <p class="z2">{{PIN}}</p>
      <input type="text" placeholder="请输入验证码" class="k2" style="outline:none;">
      <hr class="hr3" color="#e6e6e6" size="0.01px">
      <p class="z3">{{PW}}</p>
      <input type="text" placeholder="请输入密码" class="k3" style="outline:none;">
      <hr class="hr4" color="#e6e6e6" size="0.01px">
      <a href class="a1">{{HPIN}}</a>
      <a href class="a2">
        <button class="z4">{{LD}}</button>
      </a>
    </div>
    <div class="footer">
      <p class="f1">
        {{agree}}
        <a href class="a3">{{conesal}}</a>
      </p>
    </div>
  </div>
</template>

<script>
// import {fontsizeset} from './../views/fontsizeset.js'

export default {
  data() {
    return {
      jpg: require("../assets/状态栏.jpg"),
      registe: "忘记密码",
      jiao: require("../assets/Return.png"),
      MB: "手机",
      PIN: "验证码",
      PW: "密码",
      HPIN: "获取验证码",
      LD: "注册",
      agree: "注册代表同意",
      conesal: "《隐私条款》"
    };
  },
  methods: {
    Previous_page() {
      this.$router.go(-1);
    }
  }
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
}
.jpg {
  float: left;
  width: 7.5rem;
  margin-left:0.1rem;
}
.Header {
  width: 7.65rem;
  height: 0.9rem;
  background-color: black;
  float: left;
  margin-left: -0.15rem;
  /* margin-top: 0.25rem; */
}
.Header .jiao {
  float: left;
  width: 0.15rem;
  height: 0.3rem;
  margin-top: 0.1rem;
  margin-left: 0.3rem;
}
.Header .zhu {
  margin-top: 0.28rem;
  margin-left: 3.25rem;
  font-size: 0.31rem;
  color: white;
}
.body .hr1 {
  float: left;
  margin-top: 0.45rem;
  margin-left: 0.3rem;
  width: 6.91rem;
}
.body .k1 {
  float: left;
  font-size: 0.29rem;
  border: none;
  margin-top: 0.5rem;
  margin-left: 0.63rem;
  opacity: 0.55;
}
.body .z1 {
  float: left;
  font-size: 0.29rem;
  margin-left: 0.3rem;
  margin-top: 0.47rem;
}
.body .hr2 {
  float: left;
  margin-top: 0.21rem;
  margin-left: 0.3rem;
  width: 6.91rem;
}
.body .z2 {
  float: left;
  font-size: 0.29rem;
  margin-left: 0.24rem;
  margin-top: 0.47rem;
}
.body .k2 {
  float: left;
  font-size: 0.29rem;
  border: none;
  margin-top: 0.5rem;
  margin-left: 0.4rem;
  opacity: 0.55;
}
.body .hr3 {
  float: left;
  margin-top: 0.21rem;
  margin-left: 0.3rem;
  width: 6.91rem;
}
.body .z3 {
  float: left;
  font-size: 0.29rem;
  margin-left: 0.2rem;
  margin-top: 0.47rem;
}
.body .k3 {
  float: left;
  font-size: 0.29rem;
  border: none;
  margin-top: 0.5rem;
  margin-left: 0.7rem;
  opacity: 0.55;
}
.body .hr4 {
  float: left;
  margin-top: 0.21rem;
  margin-left: 0.3rem;
  width: 6.91rem;
}
.body .a1 {
  float: left;
  text-decoration: none;
  font-size: 0.29rem;
  color: #0091ff;
  margin-left: 5.7rem;
  margin-top: -1.7rem;
}
.body .z4 {
  float: left;
  width: 6.9rem;
  height: 0.88rem;
  background-color: #0091ff;
  border: 0px solid #0091ff;
  margin-top: 0.35rem;
  margin-left: 0.45rem;
  font-size: 0.29rem;
  color: white;
  border-radius: 0.05rem;
}
.footer .f1 {
  float: left;
  font-size: 0.29rem;
  margin-top: 6.78rem;
  margin-left: 2.23rem;
}
.footer .f1 .a3 {
  text-decoration: none;
  color: #0091ff;
}
</style>
