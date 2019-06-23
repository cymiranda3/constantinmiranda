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

        <b-modal id="saas-modal" ref="saas-modal" size="xl" scrollable>
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
                <li>Moore House (Student Government): House Head</li>
                <li>Headmaster's Award: 2015 & 2016 Recipient</li>
              </ul>
            </p>
            <p>The greatest aspect of Saint Anselm's, in my mind, was the level of trust in their students. As a teenager, I was given the opportunity to take charge of several high-value projects, including the development of an all-digital registration site for the ski club, the Yearbook budget and timeline, and the planning of various student government sponsored events.</p>
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

        <b-modal id="cornell-modal" ref="cornell-modal" size="xl" scrollable>
          <h3 class="modalHeader">Cornell University</h3>
          <h4 class="modalSubheader">High above Cayuga's waters...</h4>
          <b-img class="modalImage" :src="require('@/assets/images/clocktower.jpg')"></b-img>
          <div class="modalText">
            <p>I am a student in Cornell's College of Arts & Sciences and am majoring in Information Science with a User Experience concentration. I have also completed the Business Minor offered through the Dyson School of Businesss.</p>
            <p>I am a member of the Cornell University Ski Team and enjoy skiing at Greek Peak, a local mountain, during my time off. I have also really enjoyed working as a teaching assistant in the Information Science Department. I have TA'd INFO 1300, INFO 2300, and will be TA'ing INFO 4340 this coming Fall.</p>
            <p>I have also served as the president of my fraternity, Chi Phi. I have worked extremely hard to institute culture change within my chapter and am very proud of the work I have done. For the first time in our Chapter's history, the undergraduates will be funding a house improvement project in Summer 2019. We have also become extremely involved in our community, earning the highest philanthropy participation tier this past year, an honor which we share with only two other campus organizations.</p>
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

        <b-modal id="bm-modal" ref="bm-modal" size="xl" scrollable>
          <h3 class="modalHeader">Bryn Mawr: Russian Language Institute</h3>
          <h4 class="modalSubheader">Summer 2015</h4>
          <b-img class="modalImage" :src="require('@/assets/images/rli-schedule.png')"></b-img>
          <div class="modalText">
            <p>During Summer 2015, I attended Bryn Mawr's Russian Language Institute. This intensive program places students in a completely immersive environment. From day one, all classes are taught completely in Russian. Students are expected to converse with professors, teaching assistants, and peers completely in Russian. Meals were centered around specific topics relevant to our studies and are also conducted completely in Russian.Over the course of the 8 weeks, we also went on cultural trips to Washington, DC and Brighton Beach, NY, a neighborhood of New York City where a significant Russian population lives.</p>
            <p>Though this is primarily a summer program for college students, a select number of high schoolers are also admitted. As such, I found myself in a highly academic environment mirroring what I would ultimately find at Cornell. As a heritage speaker, I was able to begin at the intermediate level. Though, there was a significant learning curve for me those first few weeks as I caught up on the basic grammatical, spelling, and reading skills that my peers had already developed in prior classes.</p>
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
  width: 100%;
  margin-left: auto;
  margin-right: auto;
}

.card {
  padding: 20px;
  min-height: 25vw;
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
