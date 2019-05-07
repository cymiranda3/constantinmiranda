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

        <b-modal id="git-modal" ref="git-modal" size="xl" scrollable>
          <h3 class="modalHeader">Experience with Git</h3>
          <h4 class="modalSubheader">Cornell's Information Science Department heavily integrates the Git workflow into coursework.</h4>
          <b-img class="modalImage" :src="require('@/assets/images/git-staff.png')"></b-img>
          <div class="modalText">
            <p>Many of Cornell's courses use Github to host course repositories and individual student repositories. I've used the Git workflow both as a student, to submit my assignments in classes like INFO 2300 and 4340, and as a teaching assistant, to fetch and checkout student work for grading.</p>
            <p>I am familiar with popular Git workflow features like commits, merging commits, and using a feature-centric branch strategy.</p>
          </div>

          <div class="relevantCourses">
            <p class="rcHeader">Relevant Courses: </p>
            <p class="rcItem">INFO 2300 - Intermediate Web Design & Development</p>
            <p class="rcItem">INFO 3300 - Data Driven Web Applications</p>
            <p class="rcItem">INFO 4340 - UX & Software Development Studio</p>
            <p class="rcItem">INFO 4910 - Teaching in Information Science</p>
          </div>
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

/* Modal CSS: */
.modalHeader {
  font-family: "Old Standard Regular";
  font-size: 4vw;
}

.modalSubheader {
  font-family: "Roboto Light"
}

.modalImage {
  width: 40vw;
  margin-top: 2vw;
  border: 0.5px solid lightgray;
  border-radius: 5px;
}

.modalText {
  width: 70%;
  margin-left: auto;
  margin-right: auto;
  text-align: justify;
  margin-top: 2vw;
  font-family: "Roboto Light";
  font-size: 1.75vw;
}

.relevantCourses {
  text-align: left;
  width: 70%;
  margin-left: auto;
  margin-right: auto;
  margin-top: 3vw;
}

.rcHeader {
  font-family: "Old Standard Regular";
  font-size: 2vw;

  margin-bottom: 0px;
}

.rcItem {
  font-family: "Roboto Thin";
  font-size: 1.2vw;
}
</style>
