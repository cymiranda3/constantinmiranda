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
          <b-img class="modalImage" :src="require('@/assets/images/commit-network.png')"></b-img>
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
          v-on:click="showModal('sql-modal')"
          title=""
          :img-src="require('@/assets/images/sql.png')"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
          >
        </b-card>

        <b-modal id="sql-modal" ref="sql-modal" size="xl" scrollable>
          <h3 class="modalHeader">Experience with SQL</h3>
          <h4 class="modalSubheader"></h4>
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
          v-on:click="showModal('vue-modal')"
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

        <b-modal id="vue-modal" ref="vue-modal" size="xl" scrollable>
          <h3 class="modalHeader">Experience with Vue</h3>
          <h4 class="modalSubheader">My frontend framework of choice.</h4>
          <b-img class="modalImage" :src="require('@/assets/images/vue-countdown.png')"></b-img>
          <div class="modalText">
            <p>I've worked with several popular frontend frameworks, but Vue is by far my favorite. I like how simple it is. Someone who knows the basics of web development (HTML, JavaScript, and CSS) can become familiar with Vue's syntax and structure in a matter of hours. This is important when it comes time to expanding a project team. </p>
            <p>I'd also add that Vue's development team has done an excellent job of maintaining that focus on simplicity. For example, Vue 3.0 will make Vue even faster, even smaller, and even more maintainable. With that being said, using Vue in conjunction with Node Package Manager (NPM) means that additional functionality or complexity can very easily be added as needed.</p>
            <p>The best feature by far is the Progressive Web Application (PWA) support. PWAs are becoming more widely supported <a href="https://medium.com/@firt/progressive-web-apps-on-ios-are-here-d00430dee3a7">(here)</a> and offer the advantage of developing one code base that can then be slightly modified to be used as a desktop application, mobile application, or typical browser-acessed website.
            </p>
          </div>

          <div class="relevantCourses">
            <p class="rcHeader">Relevant Courses & Experiences: </p>
            <p class="rcItem">INFO 4340 - UX & Software Development Studio</p>
            <p class="rcItem">eLab - Noozit: Frontend Framework</p>
            <p class="rcItem">Personal Website: This site is built on Vue.</p>
          </div>
        </b-modal>
      </b-col>

      <b-col md="3">
        <b-card
          v-on:click="showModal('php-modal')"
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

        <b-modal id="php-modal" ref="php-modal" size="xl" scrollable>
          <h3 class="modalHeader">Experience with PHP</h3>
          <h4 class="modalSubheader">The joke is always that 'everyone hates PHP'.</h4>
          <b-img class="modalImage" :src="require('@/assets/images/uploadr-singleimage.png')"></b-img>
          <div class="modalText">
            <p>I have worked with PHP both as a student and as an instructor in INFO 2300. INFO 2300 seeks to build upon the skills learned in INFO 1300 by introducing students to server-side programming.</p>
            <p>Students learn to build dynamic websites and the course covers:
                <ul>
                  <li>PHP Templates</li>
                  <li>Displaying PHP Output</li>
                  <li>Filtering Input & Escaping Output with PHP</li>
                  <li>PDO Prepared Statements with SQL Databases</li>
                  <li>PHP User Sessions (implemented manually)</li>
                </ul>
            </p>
            <p></p>
          </div>

          <div class="relevantCourses">
            <p class="rcHeader">Relevant Courses & Experiences: </p>
            <p class="rcItem">INFO 2300 - Intermediate Web Design & Development (student + instructor)</p>
          </div>
        </b-modal>
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
}

.border {
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

li {
  font-size: 1.25vw;
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
