<template>
  <div class="skillcards">
    <b-card
      v-on:click="showModal('git-modal')"
      title=""
      :img-src="require('@/assets/images/git.png')"
      img-alt="Image"
      img-top
      tag="article"
      class="mb-2"
    >
    </b-card>

    <b-modal
      id="git-modal"
      ref="git-modal"
      size="xl"
      scrollable
      ok-only
      ok-variant="primary"
      ok-title="Close"
    >
      <div class="modalBody">
        <h3 class="modalHeader">Experience with Git</h3>
        <h4 class="modalSubheader">
          Cornell's Information Science Department heavily integrates the Git
          workflow into coursework.
        </h4>
        <b-img
          class="modalImage"
          :src="require('@/assets/images/commit-network.png')"
        ></b-img>
        <div class="modalText">
          <p>
            Many of Cornell's courses use Github to host course repositories and
            individual student repositories. I've used the Git workflow both as
            a student, to submit my assignments in classes like INFO 2300 and
            4340, and as a teaching assistant, to fetch and checkout student
            work for grading.
          </p>
          <p>
            I am familiar with popular Git workflow features like commits,
            merging commits, and using a feature-centric branch strategy.
          </p>
        </div>

        <div class="relevantCourses">
          <p class="rcHeader">Relevant Courses:</p>
          <p class="rcItem">
            INFO 2300 - Intermediate Web Design & Development
          </p>
          <p class="rcItem">INFO 3300 - Data Driven Web Applications</p>
          <p class="rcItem">INFO 4340 - UX & Software Development Studio</p>
          <p class="rcItem">INFO 4910 - Teaching in Information Science</p>
        </div>
      </div>
    </b-modal>

    <b-card
      v-on:click="showModal('sql-modal')"
      title=""
      :img-src="require('@/assets/images/sql.png')"
      img-alt="Image"
      img-top
      tag="article"
      class="mb-2"
    >
    </b-card>

    <b-modal
      id="sql-modal"
      ref="sql-modal"
      size="xl"
      scrollable
      ok-only
      ok-variant="primary"
      ok-title="Close"
    >
      <div class="modalBody">
        <h3 class="modalHeader">Experience with SQL</h3>
        <h4 class="modalSubheader"></h4>
        <b-img
          class="modalImage"
          :src="require('@/assets/images/db-browser.png')"
        ></b-img>
        <div class="modalText">
          <p>
            I've worked with MySQL, SQLite, and PostgreSQL in several of my
            Information Science classes. INFO 2300's final project required the
            design and implementation of a SQLite database for a complex website
            (user authentication, image storage, and form capture).
          </p>
          <p>
            I've also worked with SQL in a professional setting at Strategic
            Investment Group.
          </p>
        </div>

        <div class="relevantCourses">
          <p class="rcHeader">Relevant Courses:</p>
          <p class="rcItem">
            INFO 2300 - Intermediate Web Design & Development
          </p>
          <p class="rcItem">INFO 4910 - Teaching in Information Science</p>
        </div>
      </div>
    </b-modal>

    <b-card
      v-on:click="showModal('vue-modal')"
      title=""
      :img-src="require('@/assets/images/vue.png')"
      img-alt="Image"
      img-top
      tag="article"
      class="mb-2"
    >
    </b-card>

    <b-modal
      id="vue-modal"
      ref="vue-modal"
      size="xl"
      scrollable
      ok-only
      ok-variant="primary"
      ok-title="Close"
    >
      <div class="modalBody">
        <h3 class="modalHeader">Experience with Vue</h3>
        <h4 class="modalSubheader">My frontend framework of choice.</h4>
        <b-img
          class="modalImage"
          :src="require('@/assets/images/vue-countdown.png')"
        ></b-img>
        <div class="modalText">
          <p>
            I've worked with several popular frontend frameworks, but Vue is by
            far my favorite. Someone who knows the basics of web development
            (HTML, JavaScript, and CSS) can become familiar with Vue's syntax
            and structure in a matter of hours. This is important when it comes
            time to expanding a project team.
          </p>
          <p>
            I'd also add that Vue's development team has done an excellent job
            of maintaining that focus on simplicity. For example, Vue 3.0 will
            make Vue even faster, even smaller, and even more maintainable. With
            that being said, using Vue in conjunction with Node Package Manager
            (NPM) means that additional functionality or complexity can very
            easily be added as needed.
          </p>
          <p>
            The best feature by far is the Progressive Web Application (PWA)
            support. PWAs are becoming more widely supported
            <a
              href="https://medium.com/@firt/progressive-web-apps-on-ios-are-here-d00430dee3a7"
              >(article)</a
            >
            and offer the advantage of developing one code base that can then be
            slightly modified to be used as a desktop application, mobile
            application, or typical browser-accessed website.
          </p>
        </div>

        <div class="relevantCourses">
          <p class="rcHeader">Relevant Courses & Experiences:</p>
          <p class="rcItem">INFO 4340 - UX & Software Development Studio</p>
          <p class="rcItem">eLab - Noozit: Frontend Framework</p>
          <p class="rcItem">Personal Website: This site is built on Vue.</p>
        </div>
      </div>
    </b-modal>

    <b-card
      v-on:click="showModal('php-modal')"
      title=""
      :img-src="require('@/assets/images/php.png')"
      img-alt="Image"
      img-top
      tag="article"
      class="mb-2"
    >
    </b-card>

    <b-modal
      id="php-modal"
      ref="php-modal"
      size="xl"
      scrollable
      ok-only
      ok-variant="primary"
      ok-title="Close"
    >
      <div class="modalBody">
        <h3 class="modalHeader">Experience with PHP</h3>
        <h4 class="modalSubheader">
          The joke is always that 'everyone hates PHP'.
        </h4>
        <b-img
          class="modalImage"
          :src="require('@/assets/images/uploadr-singleimage.png')"
        ></b-img>
        <div class="modalText">
          <p>
            I have worked with PHP both as a student and as an instructor in
            INFO 2300. INFO 2300 seeks to build upon the skills learned in INFO
            1300 by introducing students to server-side programming.
          </p>
          <p>Students learn to build dynamic websites and the course covers:</p>
          <div>
            <ul>
              <li>PHP Templates</li>
              <li>Displaying PHP Output</li>
              <li>Filtering Input & Escaping Output with PHP</li>
              <li>PDO Prepared Statements with SQL Databases</li>
              <li>PHP User Sessions (implemented manually)</li>
            </ul>
          </div>
        </div>

        <div class="relevantCourses">
          <p class="rcHeader">Relevant Courses & Experiences:</p>
          <p class="rcItem">
            INFO 2300 - Intermediate Web Design & Development (student +
            instructor)
          </p>
        </div>
      </div>
    </b-modal>

    <b-card
      title=""
      :img-src="require('@/assets/images/python.png')"
      img-alt="Image"
      img-top
      tag="article"
      class="mb-2"
    >
    </b-card>

    <b-card
      title=""
      :img-src="require('@/assets/images/figma.png')"
      img-alt="Image"
      img-top
      tag="article"
      class="mb-2"
    >
    </b-card>

    <b-card
      title=""
      :img-src="require('@/assets/images/css.png')"
      img-alt="Image"
      img-top
      tag="article"
      class="mb-2"
    >
    </b-card>

    <b-card
      title=""
      :img-src="require('@/assets/images/js.png')"
      img-alt="Image"
      img-top
      tag="article"
      class="mb-2"
    >
    </b-card>
  </div>
</template>

<script>
export default {
  name: "SkillCards",
  props: {
    msg: String,
    image_path: String
  },
  methods: {
    getImage() {
      return "@/assets/images/saas.png";
    },
    showModal(id) {
      this.$refs[id].show();
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.skillcards {
  margin-top: 5%;
  align-items: stretch;
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  overflow-x: auto;
  overflow-y: hidden;
}
.card {
  /*float: left;*/
  background-color: transparent;
  padding: 20px;
  margin: 10px;
  flex-basis: 20%;
  flex-grow: 0;
  flex-shrink: 0;
  transition: all 0.4s ease-in-out;
  border: none;
}

.card:hover {
  transform: scale(1.05);
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}

.card-body {
  display: none;
}

.card-img-top {
  margin-top: auto;
  margin-bottom: auto;
}

/* Modal CSS: */
.modalHeader {
  font-family: "Old Standard Regular";
  font-size: 4vw;
}

.modalSubheader {
  font-family: "Roboto Light";
}

.modalBody {
  text-align: center;
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

/* Mobile Styles: */
@media (min-device-width: 320px) and (max-device-width: 480px) {
  .card {
    border: 1px solid lightgray;
    margin-left: 10px;
    margin-right: 10px;
    padding: 50px;
    flex-basis: 80%;
  }

  .modalHeader {
    font-size: 12vw;
  }

  .modalText {
    margin-top: 30px;
    font-size: 4vw;
  }

  .modalImage {
    width: 80vw;
  }

  ul {
    width: 95%;
    margin-left: 0;
    margin-right: 5%;
  }

  li {
    font-size: 3vw;
    padding-left: 0;
  }

  .relevantCourses {
    width: 80%;
  }

  .rcHeader {
    font-size: 6vw;
  }

  .rcItem {
    font-size: 4vw;
  }
}
</style>
