<template>
  <div class="home">
    <Biography />
    <h1 class='sectionHeader'>Education</h1>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import Biography from "@/components/Biography.vue";

export default {
  name: "home",
  components: {
    Biography,
  }
};
</script>

<style scoped>
  .sectionHeader {
    font-size: 5vw;
    font-family: "Old Standard Regular";
    color: black;
    text-align: left;
    margin-left: 40px;
  }
</style>
