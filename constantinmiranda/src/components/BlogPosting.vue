<template>
    <b-card no-body class="overflow-hidden singlePost">
      <b-row no-gutters>
        <b-col md="6">
          <b-card-img src="https://picsum.photos/400/400/?image=20" class="rounded-0"></b-card-img>
        </b-col>
        <b-col md="6">
          <b-card-body :title='blogTitle'>
            <b-card-text>
              {{ blogSubtitle }}
            </b-card-text>
          </b-card-body>
        </b-col>
      </b-row>
      <b-button class="moduleLinkButton" href="#" variant="primary">Go somewhere</b-button>
    </b-card>
</template>

<script>
export default {
  name: "BlogPosting",
  props: {
    blogImage: String,
    blogTitle: String,
    blogSubtitle: String,
    blogDate: String,
    blogBody: String,
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}

/* Styling for blog post card from here on: */
.singlePost {
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
}
.moduleLinkButton {
  border-radius: 0px 0px 5px 5px;
}
</style>
