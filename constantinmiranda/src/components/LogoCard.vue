<template>
  <div class="logocard">
    <h1>{{ getImage(image_path) }}</h1>
    <!-- <b-card
      title="Card Title"
      :img-src="getImage(image_path)"
      img-alt="Image"
      img-top
      tag="article"
      style="max-width: 20rem;"
      class="mb-2"
    > -->
    <b-card-text>
      Some quick example text to build on the card title and make up the bulk of the card's content.
    </b-card-text>

    <b-button href="#" variant="primary">Go somewhere</b-button>
  </b-card>
  </div>
</template>

<script>
export default {
  name: "LogoCard",
  props: {
    msg: String,
    image_path: String
  },
  methods:{
    getImage(image_path) {
      return require(image_path)
    }
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


</style>
