<template>
  <div class="container">
    svg1
    <input type="checkbox" name id v-model="type" />
    <div data-name="sss" >6666</div>
    <div class="scene_door" v-html="svg_src" ></div>
    <!-- <img src="~/assets/aaa.svg"/> -->
  </div>
</template>

<script>
import axios from "axios";
export default {
  // layout: "blog",
  data() {
    return {
      svg_src: "xxx",
      type: false
    };
  },
  asyncData(context) {
    console.log(context.env);
    return axios({
      method: "get",
      url:
        "http://awiclass.monoame.com/api/command.php?type=get&name=scene_door.svg"
    }).then(function(response) {
      return { svg_src: response.data };
      error(context);
    });
  },
  mounted: function() {
    // let url =
    //   "http://awiclass.monoame.com/api/command.php?type=get&name=scene_door.svg";
    // // console.log($.get(url) )
    // $.get(url, function(res) {
    //   console.log(res);
    //   this.svg_src = res;
    // });
  },
  methods: {}
};
</script>

<style  scoped >
.scene_door {
  width: 550px;
  /* background-image: url('/assets/aaa.svg'); */
}

/* g[data-name="island_1"]{
  opacity: 0;
} */

.scene_door [data-name="island_1"]{
  opacity: 0;
}
</style>
