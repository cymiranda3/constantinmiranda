<template>
  <div class="educationcards">
    <b-row id="row1">
      <b-col md="3">
        <b-card
          v-on:click="showModal('git-modal')"
          title=""
          :img-src="require('@/assets/images/git.png')"
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

        <b-modal id="git-modal" ref="git-modal" size="xl" scrollable title="Git">
          <h3></h3>
          <p class="my-4">Hello from modal!</p>
        </b-modal>

      </b-col>



      <b-col md="3">
        <b-card
          title=""
          :img-src="require('@/assets/images/django.png')"
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

      <b-col md="3">
        <b-card
          title=""
          :img-src="require('@/assets/images/vue.png')"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
          >

          <!-- <b-button href="#" variant="primary">Go somewhere</b-button> -->
        </b-card>
      </b-col>

      <b-col md="3">
        <b-card
          title=""
          :img-src="require('@/assets/images/php.png')"
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

    <b-row id="row1">
      <b-col md="3">
        <b-card
          title=""
          :img-src="require('@/assets/images/python.png')"
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

      <b-col md="3">
        <b-card
          title=""
          :img-src="require('@/assets/images/figma.png')"
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

      <b-col md="3">
        <b-card
          title=""
          :img-src="require('@/assets/images/css.png')"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
          >

          <!-- <b-button href="#" variant="primary">Go somewhere</b-button> -->
        </b-card>
      </b-col>

      <b-col md="3">
        <b-card
          title=""
          :img-src="require('@/assets/images/js.png')"
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
  name: "SkillCards",
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
    },
    showModal(id) {
      this.$refs[id].show()
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
  min-height: 20vw;
  transition: all .5s ease-in-out;
}

.card:hover {
  transform: scale(1.05);
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
