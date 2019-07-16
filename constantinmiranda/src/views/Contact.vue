<template>
  <div class="about">
    <h1>Send me an email at </h1>
    <b-button variant="primary" v-clipboard:copy="thingToCopy" v-on:click="copySuccess=true">
      cym8@cornell.edu <b-badge v-if="copySuccess" variant="light">Copied!</b-badge>
    </b-button>
  </div>
</template>

<script>
import VueClipboard from 'vue-clipboard2'
export default {
  name: "Contact",
  data() {
    return {
      copySuccess: false,
      thingToCopy: `cym8@cornell.edu`
    }
  },
  props: {
    msg: String
  }
};
</script>

<style scoped>
  .about {
    color: black;
    margin-top: 10%;
    width: 70vw;
    margin-right: auto;
    margin-left: auto;
  }
  h1 {
    margin: 0;
    font-family: "Old Standard Regular";
  }
  button {
    /* background-color: transparent; */
    /* color: black; */
    font-family: "Roboto Thin";
    border: 1px solid white;
    border-radius: 5px;
    margin-left: auto;
    margin-right: auto;
    font-size: 3vw;
  }

  span.badge {
    position: relative;
    top: -.3vw;
  }

  /* button:hover {
    background-color: black;
    color: white;
  } */


</style>
