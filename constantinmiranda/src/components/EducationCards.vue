<template>
  <div class="educationcards">
    <b-row id="row1">
      <b-col md="4">
        <b-card
          title=""
          :img-src="require('@/assets/images/saas.png')"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
          >
          <!-- <b-card-text>
            Some quick example text to build on the card title and make up the bulk of the card's content.
          </b-card-text> -->
          <!-- <b-button href="#" variant="primary">Go somewhere</b-button> -->
        </b-card>
      </b-col>

      <b-col md="4">
        <b-card
          title=""
          :img-src="require('@/assets/images/cornell.png')"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
          >
          <!-- <b-card-text>
            Some quick example text to build on the card title and make up the bulk of the card's content.
          </b-card-text> -->
          <!-- <b-button href="#" variant="primary">Go somewhere</b-button> -->
        </b-card>
      </b-col>

      <b-col md="4">
        <b-card
          title=""
          :img-src="require('@/assets/images/brynmawr.png')"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
          >

          <!-- <b-button href="#" variant="primary">Go somewhere</b-button> -->
        </b-card>
      </b-col>

    </b-row>

  </div>
</template>

<script>

export default {
  name: "EducationCards",
  props: {
    msg: String,
    image_path: String
  },
  onMount() {

    console.log(image_path)
  },
  methods:{
    getImage() {
      return '@/assets/images/saas.png'
    }
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.educationcards {
  width: 100%;
  margin-left: auto;
  margin-right: auto;
}

.card {
  padding: 20px;
  min-height: 25vw;
}

.card-body {
  display: none;
}

.card-img-top {
  margin-top: auto;
  margin-bottom: auto;
}

#row1 {
  align-items: center;
  align-content: center;
}
</style>
