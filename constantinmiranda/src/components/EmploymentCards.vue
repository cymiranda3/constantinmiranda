<template>
  <div class="employmentcards">
    <b-row id="row1">
      <b-col md="4">
        <b-card
          v-on:click="showModal('sultana-modal')"
          title=""
          :img-src="require('@/assets/images/sultana.png')"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2"
          >
        </b-card>

        <b-modal id="sultana-modal" ref="sultana-modal" size="xl" scrollable ok-only ok-variant="primary" ok-title="Close">
          <h3 class="modalHeader">Sultana Education Foundation</h3>
          <h4 class="modalSubheader">Summers 2016 & 2017</h4>
          <b-img class="modalImage" :src="require('@/assets/images/teaching.jpg')"></b-img>
          <div class="modalText">
            <p>For summers 2016 and 2017, I worked as a Paddling Staff Member for the Sultana Education Foundation. Sultana is a nonprofit organization in Chestertown, MD (Maryland's Eastern Shore). Their focus is "Preservation Through Education" and the foundation seeks to ensure the future protection and preservation of the Chesapeake Bay by educating students about the diverse flora and fauna.</p>
            <p>During my time at Sultana, I was responsible for the well-being, education, and leadership of 15-20 students. The program included both day and overnight excursions. I was certified as an American Red Cross Lifeguard and in CPR/AED.</p>
          </div>

          <!-- <div class="relevantCourses">
            <p class="rcHeader">Relevant Courses: </p>
            <p class="rcItem">INFO 2300 - Intermediate Web Design & Development</p>
            <p class="rcItem">INFO 3300 - Data Driven Web Applications</p>
            <p class="rcItem">INFO 4340 - UX & Software Development Studio</p>
            <p class="rcItem">INFO 4910 - Teaching in Information Science</p>
          </div> -->
        </b-modal>
      </b-col>


      <b-col md="4">
        <b-card
          v-on:click="showModal('ff-modal')"
          title=""
          :img-src="require('@/assets/images/ff.jpeg')"
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

        <b-modal id="ff-modal" ref="ff-modal" size="xl" scrollable ok-only ok-variant="primary" ok-title="Close">
          <h3 class="modalHeader">Farther Farms</h3>
          <h4 class="modalSubheader">Summer 2018</h4>
          <b-img class="modalImage" :src="require('@/assets/images/ff-website.jpg')"></b-img>
          <div class="modalText">
            <p>During Summer 2018, I worked as a Business Development Intern for Farther Farms, a startup out of Cornell's entrepreneurship program. Farther Farms is working on creating the "never frozen french fry". Some of my duties included:<p>
            <p>
              <ul>
                <li>Creating a weekly report on industry news and findings.</li>
                <li>Researching prospective sales opportunities.</li>
                <li>Researching and presenting on trends in the food industry.</li>
                <li>Researching and analyzing industry patent holdings.</li>
                <li>Participating in diligence meetings with prospective investors.</li>
                <li>Building out website functionality, such as their email capture form (live on <a href="http://www.fartherfarms.com/">their website).</a></li>
                <li>Processing potatos for test production runs.</li>
                <li>Taste testing.</li>
              </ul>
            </p>
            <p>At Farther Farms, I had the opportunity to pitch in on a wide variety of projects and apply my skills where I was most needed. The small team setting meant that I worked directly with the CEO, CTO, and VP of Business Development on a daily basis.</p>
          </div>
        </b-modal>
      </b-col>

      <b-col md="4">
        <b-card
          v-on:click="showModal('strategic-modal')"
          title=""
          :img-src="require('@/assets/images/strategic.png')"
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

        <b-modal id="strategic-modal" ref="strategic-modal" size="xl" scrollable ok-only ok-variant="primary" ok-title="Close">
          <h3 class="modalHeader">Strategic Investment Group</h3>
          <h4 class="modalSubheader">Summer 2019</h4>
          <b-img class="modalImage" :src="require('@/assets/images/strategic-interior.jpg')"></b-img>
          <div class="modalText">
            <p>I am currently completing an internship with Strategic Investment Group, based in Rosslyn, VA. I have been placed on the Fixed Income team, but will rotate through each asset class over the first 5 weeks. During the final five weeks, I will be preparing a final project to present to the entire company at the conclusion of the 10-week program.</p>
            <p>Strategic is one of the leading OCIO firms in the country. They manage $37 Billion from a wide array of clients.</p>
            <p>This page will be updated at the conclusion of the program.</p>
          </div>

          <!-- <div class="relevantCourses">
            <p class="rcHeader">Relevant Courses: </p>
            <p class="rcItem">INFO 2300 - Intermediate Web Design & Development</p>
            <p class="rcItem">INFO 3300 - Data Driven Web Applications</p>
            <p class="rcItem">INFO 4340 - UX & Software Development Studio</p>
            <p class="rcItem">INFO 4910 - Teaching in Information Science</p>
          </div> -->
        </b-modal>
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
    },
    showModal(id) {
      this.$refs[id].show()
    }
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.employmentcards {
  margin-top: 5%;
  justify-content: space-around;
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
  width: 20vw;
  height: 20vw;
  padding: 20px;
  margin: 10px;
  flex-basis: 20%;
  flex-grow: 0;
  flex-shrink: 0;
  transition: all .4s ease-in-out;
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

/* Mobile Styles: */
@media (min-device-width : 320px) and (max-device-width : 480px) {
  .card {
    width: 80vw;
    height: 80vw;
    border: 1px solid lightgray;
    margin-left: auto;
    margin-right: auto;
    padding: 50px;
    flex-basis: 80%;
  }
}
</style>
