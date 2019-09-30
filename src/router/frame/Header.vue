<template>
  <div>
      <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="#" id="title">InDesign Secrets</b-navbar-brand>
    
    <v-spacer></v-spacer>
    
    

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
  <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav class="ml-auto">
          <b-navbar-nav>
            <b-nav-item @click="redirect('/Login')" id="login">Login</b-nav-item>
            <b-nav-item @click="redirect('/Register')"  id="signup">Sign Up</b-nav-item>
          </b-navbar-nav>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>
<style scoped lang="scss">
@import "assets/colors.scss";
#title {
  color: $warning !important;
}
 #login{
          color: $warning !important;
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
