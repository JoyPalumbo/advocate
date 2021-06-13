<template>
  <v-app>
    <v-toolbar dark color="#162130" style="height: 8vh" fixed>
      <v-toolbar-title class="white--text">
        <div class="header"></div>
      </v-toolbar-title>

      <v-toolbar-items>
        <v-btn flat>Entertainment</v-btn>
        <v-btn flat>Sports</v-btn>
        <v-btn flat>Weather</v-btn>
        <v-btn flat>Food</v-btn>
        <v-btn flat>Opinion</v-btn>
      </v-toolbar-items>

      <v-spacer></v-spacer>

      <v-layout row align-center style="max-width: 30vw; min-width: 1vw">
        <v-text-field
          solo
          placeholder="Search"
          single-line
          append-icon="search"
          background-color="#202d3f"
          color="white"
          hide-details
        ></v-text-field>
      </v-layout>
    </v-toolbar>
    <div>
      <h1>The Advocate</h1>
    </div>
  </v-app>
</template>

<script>
export default {
  name: "Header",
  props: {
    msg: String,
  },
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
a {
  color: #42b983;
}
</style>

  