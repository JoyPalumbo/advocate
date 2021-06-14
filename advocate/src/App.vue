<template>
  <div id="app">
    <Header />
    <h1>The Advocate</h1>
    <!-- <ul>

    <li v-for="(item) in childData" :key="item.id">{{item.title}}</li>
    <li>meep</li>
    </ul> -->
    <Newsfeed v-on:passData="getData($event)"/>
    <v-row>
 <v-col cols="2"></v-col>
    <v-col cols="8"> 

    <Carousel />
    </v-col>
    <v-col cols="2"></v-col>
    </v-row>
  </div>
</template>



<script>
import Header from "./components/Header";
import Newsfeed from "./components/Newsfeed";
import Carousel from "./components/Carousel"

export default {
  name: "App",
  components: {
    Header,
    Newsfeed,
    Carousel
  },
  data(){
    return{
    childData: {title: "boo"}
    }
  },
  methods: {
    getData: function(data){
      console.log("in our get function", data)
      this.childData = data
    },
  
  }

  
};


</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  /* -webkit-font-smoothing: antialiased; */
  /* -moz-osx-font-smoothing: grayscale; */
  text-align: center;
  /* color: #2c3e50; */
  /* margin-top: 60px; */
}
</style>
