<template>
  <div class="container">v3333</div>
</template>

<script>
// import { load } from "recaptcha-v3";

export default {
  name: "",
  props: {},
  data: function() {
    // 資料
    return {
      src: "" //追蹤 store用
    };
  },
  watch: {
    //監聽值
  },
  computed: {
    //相依的資料改變時才做計算方法
  },
  methods: {
    // 初始
    // aaa() {
    //   const recaptcha = await load("6LdrXSkTAAAAACyXjkDFu9EuHa1_dOj5Y1H6m0Hh");
    //   const token =  await recaptcha.execute("login");

    //   console.log(token); // Will also print the token
    // }
  },
  //BEGIN--生命週期
  beforeCreate: function() {
    //實體初始化
  },
  created: function() {
    //實體建立完成。資料 data 已可取得，但 el 屬性還未被建立。
    console.log(99999999)
    // this.aaa()
  },
  beforeMount: function() {
    //執行元素掛載之前。
  },
  mounted: function() {
    //元素已掛載， el 被建立。
  },
  beforeUpdate: function() {
    //當資料變化時被呼叫，還不會描繪 View。
  },
  updated: function() {
    //當資料變化時被呼叫，還不會描繪 View。
  },
  beforeDestroy: function() {
    //實體還可使用。
  },
  destroyed: function() {
    //實體銷毀。
  }
  //END--生命週期
};
</script>

<style>
</style>
