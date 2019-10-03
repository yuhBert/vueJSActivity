<template>
  <div>
    <b-card title="Card Title" no-body>
      <b-card-header header-tag="nav">
        <b-nav card-header tabs>
          <b-nav-item active>LIT-U</b-nav-item>
          <b-nav-item @click="redirect('/Login')" id="login">Login</b-nav-item>
          <b-nav-item @click="redirect('/Register')" id="signup">Sign Up</b-nav-item>
        </b-nav>
      </b-card-header>

      <b-card-body id="background">
        <b-card-text class="text-center">LUCIFER INSTITUTE OF TECHNOLOGY UNIVERSITY</b-card-text>
      </b-card-body>
    </b-card>
  </div>
</template>
<style scoped lang="scss">
@import "assets/style.scss";
#title {
  color: $primary !important;
}

#background {
  background-color: #ffc299;
}
</style>
<script>
import ROUTER from "router";
export default {
  methods: {
    redirect(router) {
      ROUTER.push(router);
    }
  }
};
</script>
