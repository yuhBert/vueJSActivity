<template>
  <div>
    <div>
      <h1>Dashboard</h1>
    </div>
    <div id="card">
      <b-card no-body class="overflow-hidden" style="max-width: 1000px;">
        <b-card-img id="image" :src="require('assets/dash.jpg')" class="rounded-0"></b-card-img>
        <hr>
        <b-card-text class="text-center">
          <h1>Hi {{username}}</h1>
          <h3>Welcome to Lucifer Institute of Technology University</h3>
        </b-card-text>
        <hr>
      </b-card>
    </div>
  </div>
</template>

<style scoped lang="scss">
@import "assets/colors.scss";
#card {
  margin-left: $margin-left !important;
  margin-top: $margin-top !important;
}

#image {
  width: $dashwidth !important;
  height: $dashheight !important;
}
</style>

<script>
export default {
  name: "card",
  data() {
    return {
      username: sessionStorage.getItem("Username")
    };
  }
};
</script>