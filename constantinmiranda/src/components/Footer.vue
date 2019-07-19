<template>
  <div class="footer">
    <p>&copy; Constantin Miranda 2019</p>
    <p>Made in DC.</p>
  </div>
</template>

<script>
export default {
  name: "Footer",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer {
  padding-top: 10vw;
}
</style>
