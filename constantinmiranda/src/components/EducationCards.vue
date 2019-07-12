<template>
  <div class="educationcards">
    <b-row id="row1">
      <b-col md="4">
        <b-card
          v-on:click="showModal('saas-modal')"
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

        <b-modal id="saas-modal" ref="saas-modal" size="xl" scrollable ok-only ok-variant="primary" ok-title="Close">
          <h3 class="modalHeader">Saint Anselm's Abbey School</h3>
          <!-- <h4 class="modalSubheader">Cornell's Information Science Department heavily integrates the Git workflow into coursework.</h4> -->
          <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/46c4-KqRB9k?controls=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
          <!-- <b-img class="modalImage" :src="require('@/assets/images/commit-network.png')"></b-img> -->
          <div class="modalText">
            <p>Saint Anselm's is a Benedictine middle and high school located in Northeast Washington, DC. While at Saint Anselm's, I was heavily involved with a variety of activities and organizations, including:</p>
            <p>
              <ul>
                <li>Ski Club: Founder & President <a href="http://www.abbeysnowsports.com">(Website)</a></li>
                <li>Varsity Tennis: Captain</li>
                <li>Junior Varsity & Varsity Lacrosse</li>
                <li>The Priory Perspective (Yearbook): Editor-in-Chief</li>
                <li>The Priory Press (Newspaper): Photographer & Guest Contributor</li>
                <li>Film Club</li>
                <li>Student Government: Moore House Head</li>
                <li>Headmaster's Award: 2015 & 2016 Recipient</li>
              </ul>
            </p>
            <p>At Saint Anselm's, I had the opportunity to take charge of several high-value projects, including the development of an all-digital registration site for our ski club, the Priory Perspective's budget and timeline, and the planning of various student government sponsored events.</p>
          </div>
        </b-modal>
      </b-col>

      <b-col md="4">
        <b-card
          v-on:click="showModal('cornell-modal')"
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

        <b-modal id="cornell-modal" ref="cornell-modal" size="xl" scrollable ok-only ok-variant="primary" ok-title="Close">
          <h3 class="modalHeader">Cornell University</h3>
          <h4 class="modalSubheader">High above Cayuga's waters...</h4>
          <b-img class="modalImage" :src="require('@/assets/images/clocktower.jpg')"></b-img>
          <div class="modalText">
            <p>I am a student in Cornell's College of Arts & Sciences majoring in Information Science with a concentration in User Experience (UX). I have also completed the University Wide Business Minor, which is offered through the Dyson School of Businesss.</p>
            <p>I am a member of the Cornell University Ski Team and enjoy skiing at Greek Peak, a local mountain, during my time off. I've enjoyed working as a teaching assistant in the Information Science Department. I have TA'd INFO 1300, INFO 2300, and will be TA'ing INFO 4340 this coming Fall.</p>
          </div>

          <div class="relevantCourses">
            <p class="rcHeader">Selected Coursework: </p>
            <p class="rcItem">AEM 2241 - Finance</p>
            <p class="rcItem">ANTHR 2468 - Medicine, Culture, and Society</p>
            <p class="rcItem">ECON 3805 - Competition Law and Policy</p>
            <p class="rcItem">INFO 4910 - Teaching in Information Science</p>
            <p class="rcItem">INFO 4340 - UX & Software Development Studio</p>
            <p class="rcItem">INFO 3450 - Human-Computer Interaction Design/p>
            <p class="rcItem">INFO 2300 - Intermediate Web Design & Development</p>
            <p class="rcItem">INFO 2950 - Introduction to Data Science</p>
            <p class="rcItem">INFO 3300 - Data Driven Web Applications</p>
            <p class="rcItem">INFO 1200 - Information Ethics, Law, and Policy</p>
            <p class="rcItem">NBA 6230 & 6330 - Actualizing Your Startup Pts. I & II</p>
            <p class="rcItem">NES 2754 - Wondrous Literature of the Near East</p>
            <p class="rcItem">NES 2676 - Holy War, Crusade, & Jihad from Antiquity to Present</p>
            <p class="rcItem">RUSSA 3303 - Advanced Composition and Conversation</p>
            <p class="rcItem">STSCI 2100 - Introductory Statistics</p>
          </div>
        </b-modal>
      </b-col>

      <b-col md="4">
        <b-card
          v-on:click="showModal('bm-modal')"
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

        <b-modal id="bm-modal" ref="bm-modal" size="xl" scrollable ok-only ok-variant="primary" ok-title="Close">
          <h3 class="modalHeader">Bryn Mawr: Russian Language Institute</h3>
          <h4 class="modalSubheader">Summer 2015</h4>
          <b-img class="modalImage" :src="require('@/assets/images/rli-schedule.png')"></b-img>
          <div class="modalText">
            <p>During Summer 2015, I attended Bryn Mawr's Russian Language Institute. This intensive program places students in a completely immersive environment. From day one, all classes are taught completely in Russian. Students are expected to converse with professors, teaching assistants, and peers in Russian. Meals were centered around specific topics relevant to our studies and are also conducted completely in Russian. Over the course of the 8 weeks, we took cultural trips to Washington, DC and Brighton Beach, NY, a neighborhood of New York City where a significant Russian population lives.</p>
            <p>Though this is primarily a summer program for college students, a select number of high schoolers are also admitted. As such, I found myself in a highly academic environment mirroring what I would ultimately find at Cornell. As a heritage speaker, I was able to begin at the intermediate level. There was a significant learning curve for me those first few weeks as I caught up on the basic grammatical, spelling, and reading skills that my peers had already developed in prior classes.</p>
            <p>I completed the equivalent of two intermediate level college courses over eight weeks. I finished with a 4.0 GPA in both courses.</p>
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

.educationcards {
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
