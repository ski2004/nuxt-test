<template>
  <div class="container">
    <nuxt-link to="/">back</nuxt-link>
    <h1 class="title">{{title}}</h1>
    <p>{{data}}</p>
    <button @click="aa()" >aa</button>
  </div>
</template>

<script>
export default {
  // layout:"test",
  components: {
    // Logo
  },
  data() {
    return {
      title: "test  SSR",
      data:{}
    };
  },
  methods:{
    aa(params) {
      let url = `http://localhost:8000/api/post`
    this.$axios.get(url).then( res => {
      console.log(res)    
    });
    },
  },
  async asyncData ({ app }) {
    // 这里data等同于上面的res.data
    
  },
};
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
