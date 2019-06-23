<template>
  <div class="bio">
    <b-card id="bioCard" no-body class="overflow-hidden">
      <b-row no-gutters id="biographyRow">
        <b-col md="6">
          <b-card-img id="bioCardImage" :src="require('../assets/images/snowbird.jpg')" class="rounded-0"></b-card-img>
        </b-col>
        <b-col md="6">
          <b-card-body title="Currently @ Strategic Investment Group">
            <b-card-text id="biography">
              Currently a Junior at Cornell pursuing Information Science (Concentration: UX) and a Business minor. I'm interested in both the financial and technology industries. I have experience writing and working with a variety of backend (Flask - Python, Django - Python, Express - JS) and frontend (Vue, Angular, React) technologies. I also have experience working with SciKit-Learn and NumPy in Python environments and notebooks. I maintain a personal portfolio diversified across stocks, bonds, ETFs, and Mutual Funds and regularly follow market trends and events to inform my investing strategy.
            </b-card-text>
          </b-card-body>
        </b-col>
      </b-row>
    </b-card>
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
  }

  #bioCard {
    width: 100%;
    margin-left: auto;
    margin-right: auto;
  }

  #biography {
    font-size: 1.5vw;
    text-align: left;
    padding-left: 2vw;
  }

</style>
