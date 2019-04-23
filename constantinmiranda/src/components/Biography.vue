<template>
  <div class="bio">
    <b-card id="bioCard" no-body class="overflow-hidden">
    <b-row no-gutters>
      <b-col md="6">
        <b-card-img id="bioCardImage" :src="require('../assets/images/snowbird.jpg')" class="rounded-0"></b-card-img>
      </b-col>
      <b-col md="6">
        <b-card-body title="Currently @ Strategic Investment Group">
          <b-card-text>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
          </b-card-text>
        </b-card-body>
      </b-col>
    </b-row>
  </b-card>
  </div>
</template>

<script>
export default {
  name: "Biography",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .bio {
    margin-left: auto;
    margin-right: auto;
  }

  #bioCard {
    width: 70vw;
    min-width: 150px;
    margin-left: auto;
    margin-right: auto;
  }

  #bioCardImage {
    min-height: 261px;
  }

</style>
