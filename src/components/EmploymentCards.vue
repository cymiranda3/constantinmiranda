<template>
  <div class="employmentcards">
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

    <b-modal
      id="sultana-modal"
      ref="sultana-modal"
      size="xl"
      scrollable
      ok-only
      ok-variant="primary"
      ok-title="Close"
    >
      <div class="modalBody">
        <h3 class="modalHeader">Sultana Education Foundation</h3>
        <h4 class="modalSubheader">Summers 2016 & 2017</h4>
        <b-img
          class="modalImage"
          :src="require('@/assets/images/teaching.jpg')"
        ></b-img>
        <div class="modalText">
          <p>
            For summers 2016 and 2017, I worked as a Paddling Staff Member for
            the Sultana Education Foundation. Sultana is a nonprofit
            organization in Chestertown, MD (Maryland's Eastern Shore). Their
            focus is "Preservation Through Education" and the foundation seeks
            to ensure the future protection and preservation of the Chesapeake
            Bay by educating students about the diverse flora and fauna.
          </p>
          <p>
            During my time at Sultana, I was responsible for the well-being,
            education, and leadership of 15-20 students. The program included
            both day and overnight excursions. I was certified as an American
            Red Cross Lifeguard and in CPR/AED.
          </p>
        </div>
      </div>
    </b-modal>

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
    </b-card>

    <b-modal
      id="ff-modal"
      ref="ff-modal"
      size="xl"
      scrollable
      ok-only
      ok-variant="primary"
      ok-title="Close"
    >
      <div class="modalBody">
        <h3 class="modalHeader">Farther Farms</h3>
        <h4 class="modalSubheader">Summer 2018</h4>
        <b-img
          class="modalImage"
          :src="require('@/assets/images/ff-website.jpg')"
        ></b-img>
        <div class="modalText">
          <p>Farther Farms is a Cornell startup working on commercializing a novel food-preservation technology developed in Cornell University’s Department of Food Science.</p>

          <p>Duties included assisting in the company’s fundraising and diligence round, researching and 	compiling prior art for patent filings, building out website functionality for improved marketing strategies, and securing letters-of-intent from potential clients.</p>

          <p>Contract Work: Intellectual Property Research (January - March 2019): Web-scraped patent filing data and 	conducted analysis based on firm, geographic area, and filing type.</p>

        </div>
      </div>
    </b-modal>

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
    </b-card>

    <b-modal
      id="strategic-modal"
      ref="strategic-modal"
      size="xl"
      scrollable
      ok-only
      ok-variant="primary"
      ok-title="Close"
    >
      <div class="modalBody">
        <h3 class="modalHeader">Strategic Investment Group</h3>
        <h4 class="modalSubheader">Summer 2019</h4>
        <b-img
          class="modalImage"
          :src="require('@/assets/images/strategic-interior.jpg')"
        ></b-img>
        <div class="modalText">
          <p>Strategic Investment Group (SIG) is a pioneer in the outsourced chief investment office (OCIO) industry with $37 Billion in assets under management.</p>

          <p>The first five weeks consisted of a rotation through each of SIG’s asset class teams.The following five weeks focused on research and preparation for a final presentation to the firm. Opportunities included attending manager meetings, reviewing manager decks, finalizing client reporting materials, and spreadsheet modeling.</p>

          <p>Final Project & Presentation to the Firm: Evaluated SIG’s competitive position in the current OCIO landscape and identified future growth opportunities using both quantitative and qualitative data sources.</p>
        </div>
      </div>
    </b-modal>
  </div>
</template>

<script>
export default {
  name: "EducationCards",
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
  display: block;
  margin-left: auto;
  margin-right: auto;
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
  .employmentcards {
    display: inline-block;
  }
  .card {
    width: 80vw;
    height: 80vw;
    border: 1px solid lightgray;
    margin-left: auto;
    margin-right: auto;
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
