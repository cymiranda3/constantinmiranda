<template>
  <div class="navbar">
    <b-nav pills>
      <b-nav-item exact to="/">Resume</b-nav-item>
      <b-nav-item exact to="blog">Blog</b-nav-item>
      <b-nav-item>Contact</b-nav-item>
    </b-nav>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#nav a {
  font-family: "Roboto";
  font-weight: lighter;
  color: black;
}
#nav a.router-link-active {
  background-color: #eb2f06;
  color: white;
}

</style>
