<template>
  <div class="bio">
    <b-card img-src='card' img-alt="Card image" img-left class="mb-3">
      <b-card-text>
        Some quick example text to build on the card and make up the bulk of the card's content.
      </b-card-text>
    </b-card>
  </div>
</template>

<script>
import foot1 from '../assets/images/snowbird.jpg';
export default {
  name: "Biography",
  data() {
    card: foot1;
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .bio {
    width: 80vw;
    margin-left: auto;
    margin-right: auto;
  }

</style>
