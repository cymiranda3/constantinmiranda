<template>
  <div class="about">
    <h1>shoot me an email at</h1>
    <b-button  class="bounce" variant="primary" v-clipboard:copy="thingToCopy" v-on:click="copySuccess=true">
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
    font-family: "Roboto Thin";
    font-size: 4vw;
  }
  button {
    /* background-color: transparent; */
    /* color: black; */
    font-family: "Roboto Light";
    border: 1px solid white;
    border-radius: 8px;
    margin-left: auto;
    margin-right: auto;
    margin-top: 4vw;
    font-size: 3vw;
    -webkit-animation: bounce .7s 2;
  }

  span.badge {
    position: relative;
    top: -.3vw;
  }

  @-webkit-keyframes bounce {
          0% {
      transform: scale(1,1) translate(0px, 0px);
    }

    30%{
      transform: scale(1,0.8) translate(0px, 15px);
    }

    75%{
      transform: scale(1,1.1) translate(0px, -15px);
    }

   100% {
      transform: scale(1,1) translate(0px, 0px);
    }
  }

  @media (min-device-width : 320px) and (max-device-width : 480px) {
    button {
      font-size: 5vw;
      height: 70px;
      width: 70vw;
    }

    span.badge {
      border-radius: 4px;
      font-size: 5vw;
      top: -.15vw;
      vertical-align: middle;
      padding: 10px 5px;
    }
  }


</style>
