<template>
  <div class="bio">
      <b-row no-gutters id="biographyRow">
        <b-col md="6">
          <b-img id="bioImage" :src="require('../assets/images/snowbird.jpg')"></b-img>
        </b-col>
        <b-col md="6">
          <b-card-body id="biographyTitle" title="Currently @ Strategic Investment Group">
            <b-card-text id="biography">
              Currently a Junior at Cornell pursuing Information Science (Concentration: UX) and a Business minor. I'm interested in both the financial and technology industries. I have experience writing and working with a variety of backend (Flask - Python, Django - Python, Express - JS) and frontend (Vue, Angular, React) technologies. I also have experience working with SciKit-Learn and NumPy in Python environments and notebooks. I maintain a personal portfolio diversified across stocks, bonds, ETFs, and Mutual Funds and regularly follow market trends and events to inform my investing strategy.
            </b-card-text>
          </b-card-body>
        </b-col>
      </b-row>
  </div>
</template>

<script>
export default {
  name: "Biography",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .bio {
    margin-left: auto;
    margin-right: auto;
    margin-top: 8%;
  }

  #bioImage {
    display: inline-block;
    max-width: 38vw;
  }

  #biographyTitle {
    padding-left: 3vw;
  }

  #biography {
    display: inline-block;
    max-width: 38vw;
    font-size: 1.4vw;
  }

  @media (min-device-width : 320px) and (max-device-width : 480px) {
    #bioImage {
      max-width: 70vw;
    }

    #biography {
      font-size: 4vw;
      max-width: 70vw;
      padding-left: 0;
    }
  }

</style>
