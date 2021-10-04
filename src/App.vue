<template>
  <div id="app">
    
    <div class="container">
    <Navbar />
    <div class="row row-cols-1 row-cols-md-2 g-4  mt-5">
      <div class="d-flex justify-content-center col"><Card /></div>
      <div class="col ">
        <h1 class="d-flex justify-content-center">Material Dashboard </h1>
        <p class="d-flex justify-content-center"> Free bootstarp5 material Admin </p>
        <i class="bi bi-star-fill"></i>
        <p class="d-flex justify-content-center"> <star-rating
   
     v-bind:increment=".1"
     v-bind:max-rating="5"
     inactive-color="#000"
     active-color="#cc1166"
     v-bind:star-size="30"
    >
</star-rating> (1170 review)</p>
<calendar/>
      </div>
    </div>
    
    
  </div>
    
    <p class="container"> <slider/> </p>
    <h1 class="d-flex justify-content-center mb-5"> Details About Customer in Tabular Format</h1>

    <Table/>
    <Footer/>
    
    
    
    
  </div>
</template>

<script>
import StarRating from 'vue-star-rating'
import Table from './components/Table.vue'

import Calendar from './components/Calendar.vue'
import slider from './components/slider.vue'
import Navbar from './components/Navbar.vue'
import Card from './components/Card.vue'
import Footer from './components/Footer.vue'



export default {
  name: 'App',
  components: {
    
    Calendar,Table,Footer,
    slider,Navbar,Card,StarRating
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
