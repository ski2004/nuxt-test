<template>
  <div class="container">
    xxxx
    <!-- <vue-recaptcha 
      sitekey="6LdrXSkTAAAAACyXjkDFu9EuHa1_dOj5Y1H6m0Hh" 
      :loadRecaptchaScript="true"
    ></vue-recaptcha>-->
    <vue-recaptcha
          ref="recaptcha"
          @verify="onVerify"
          @expired="onExpired"
          sitekey="6LdrXSkTAAAAACyXjkDFu9EuHa1_dOj5Y1H6m0Hh">
        </vue-recaptcha>
    <button @click="resetRecaptcha"> Reset ReCAPTCHA </button>
    <!-- <form @submit.prevent="onSubmit">
      <vue-recaptcha
        ref="invisibleRecaptcha"
        @verify="onVerify"
        @expired="onExpired"
        size="invisible"
        sitekey="6LdrXSkTAAAAACyXjkDFu9EuHa1_dOj5Y1H6m0Hh"
      ></vue-recaptcha>
      <button type="submit">Submit</button>
    </form> -->
  </div>
</template>

<script>
import VueRecaptcha from "vue-recaptcha";

export default {
  layout: "blog",
  components: { VueRecaptcha },
  methods: {
    onSubmit: function() {
      this.$refs.invisibleRecaptcha.execute();
    },
    onVerify: function(response) {
      console.log("Verify: " + response);
    },
    onExpired: function() {
      console.log("Expired");
    },
    resetRecaptcha() {
      this.$refs.recaptcha.reset(); // Direct call reset method
    }
  }
};
</script>

<style>
</style>
