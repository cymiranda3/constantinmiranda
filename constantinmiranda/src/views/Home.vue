<template>
  <div class="home">
    <section class="company-heading intro-type" id="parallax-one">
      <div class="container">
        <div class="row product-title-info">
          <div class="col-md-12">
            <Biography />
            <a class="ct-btn-scroll ct-js-btn-scroll" href="#education"><img alt="Arrow Down Icon" src="https://www.solodev.com/assets/anchor/arrow-down.png"></a>
          </div>
        </div>
      </div>
      <div class="parallax" id="parallax-cta"></div>
    </section>

    <div class="main">
      <section id="education">
        <div class="container">
          <h1 class='sectionHeader'>Education</h1>
          <a class="ct-btn-scroll ct-js-btn-scroll" href="#skills"><img alt="Arrow Down Icon" src="https://www.solodev.com/assets/anchor/arrow-down.png"></a>
        </div>
      </section>

      <section id="skills">
        <div class="container">
          <h1 class='sectionHeader'>Skills</h1>
        </div>
      </section>

      <section id="work-experience">
        <div class="container">
          <h1 class='sectionHeader'>Work Experience</h1>
        </div>
      </section>
    </div>

  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import Biography from "@/components/Biography.vue";
import $ from 'jquery'

export default {
  name: "home",
  components: {
    Biography,
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
    margin-left: 40px;
  }

  .sectionWrapper {
    margin-top: 3vw;
    margin-bottom: 18vh;
  }

  /* For scrolling */
  .intro-type .container {
    padding: 107px 0px 102px 0px !important;
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

  .ct-btn-scroll {
    color: black;
    width: 49px;
    height: 49px;
    position: relative;
    bottom: 30px;
    left: 0;
    right: 0;
    top: -20px;
    margin: auto;
    padding-top: 500px;
    z-index: 9;
    border-radius: 50%;
    -webkit-transition: background-color 0.25s ease-in-out;
    transition: background-color 0.25s ease-in-out;
  }

  img,
  figure {
    max-width: 100%;
  }

  #education, #skills, #work-experience {
    height: 100vh;
    padding-top: 30px;
  }
</style>
