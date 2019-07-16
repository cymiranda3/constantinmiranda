<template>
  <div class="home">
    <section class="company-heading" id="parallax-one">
      <div class="container">
        <div class="row product-title-info">
          <div class="col-md-12">
            <Biography />
            <!-- <a class="btn-main ct-btn-scroll ct-js-btn-scroll" href="#education"><img class="sectionArrow" alt="Arrow Down Icon" :src="require('../assets/images/down-arrow.png')"></a> -->
          </div>
        </div>
      </div>
      <div class="parallax" id="parallax-cta"></div>
    </section>

    <div class="main">
      <section id="education">
        <div class="container">
          <h1 class='sectionHeader'>Education</h1>
          <EducationCards />
          <!-- <a class="ct-btn-scroll ct-js-btn-scroll" href="#skills"><img class="sectionArrow" alt="Arrow Down Icon" :src="require('../assets/images/down-arrow.png')"></a> -->
        </div>
      </section>

      <section id="skills">
        <div class="container">
          <h1 class='sectionHeader'>Skills</h1>
          <SkillCards id="skillcards"/>
        </div>
      </section>

      <section id="work-experience">
        <div class="container">
          <h1 class='sectionHeader'>Work Experience</h1>
          <EmploymentCards />
        </div>
      </section>
    </div>
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import Biography from "@/components/Biography.vue";
import EducationCards from "@/components/EducationCards.vue"
import SkillCards from "@/components/SkillCards.vue"
import EmploymentCards from "@/components/EmploymentCards.vue"
import Footer from "@/components/Footer.vue"
import $ from 'jquery'

export default {
  name: "home",
  components: {
    Biography,
    EducationCards,
    SkillCards,
    EmploymentCards,
    Footer
  },
  mounted: function() {
    $("a").on('click', function(event) {
      if (this.hash !== "") {
        event.preventDefault();
        var hash = this.hash;
        $('html, body').animate({
          scrollTop: $(hash).offset().top
        }, 800, function(){
          window.location.hash = hash;
        });
      }
    });
  }
};
</script>

<style scoped>
  .sectionHeader {
    font-size: 5vw;
    font-family: "Old Standard Regular";
    color: black;
    text-align: left;

  }

  .sectionWrapper {
    margin-top: 3vw;
    margin-bottom: 18vh;
  }

  /* For scrolling */
  .intro-type .container {
    padding: 1vw 0vw;
  }

  #parallax-one {
    display: block;
    margin-bottom: 10%;
  }

  .parallax {
    background-attachment: inherit !important;
    background-repeat: repeat;
    background-size: cover;
    position: absolute;
    top: 0px;
    bottom: 0px;
    width: 100%;
    z-index: -10;
  }

  .btn-main {
    position: absolute;
    bottom: -200px;
  }

  .ct-btn-scroll {
    padding: 10vw 0px;
    display: block;
    width: 100%;
    margin-left: auto;
    margin-right: auto;
    z-index: 9;
    -webkit-transition: background-color 0.25s ease-in-out;
    transition: background-color 0.25s ease-in-out;
  }

  img,
  figure {
    max-width: 100%;
  }

  #education, #skills, #work-experience {
    height: 40vw;
    padding-top: 30px;
  }

  .sectionArrow {
    height: 50px;
    width: 50px;
  }

  @media (min-device-width : 320px) and (max-device-width : 480px) {
    .sectionHeader {
      font-size: 10vw;
      margin-left: 1vw;
    }

    #skills {
      height: 60vh;
      display: block;
    }

    #education {
      height: 160vh;
      margin-bottom: 8vh;
      margin-top: 10vh;
      display: block;
    }

    #skillcards {
      margin-top: 10vw;
    }

}
</style>
