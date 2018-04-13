<template lang="pug">
  div#app
    pre {{crypt.genSaltSync(10)}}
    router-view

</template>

<script>
import bcrypt from "bcryptjs";

export default {
  name: "helper",
  data() {
    return {
      crypt: bcrypt
    };
  }
};
</script>

<style>
/* CSS */
</style>
