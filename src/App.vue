<template>
  <v-app>
    <Header/>
    <div class="wrapper">
      <v-container class="grey lighten-5">
        <v-row no-gutters dense>
          <v-col cols="5">
            <Map/>
          </v-col>
          <v-col cols="2">
            <Stamina/>
          </v-col>
          <v-col cols="2">
            <Point/>
          </v-col>
          <v-col cols="3">
            <Inventory/>
          </v-col>
        </v-row>
        <v-row no-gutters dense>
          <v-col cols="5">
            <Status/>
          </v-col>
          <v-col cols="3">
            <Turn/>
          </v-col>
          <v-col cols="4">
            <Armor/>
          </v-col>
        </v-row>
        <v-row no-gutters>
          <v-col cols="12">
            <Footer/>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </v-app>
</template>

<script>
import Header from './components/Header'
import Map from './components/Map'
import Stamina from "@/components/Stamina";
import Point from "@/components/Point";
import Inventory from "@/components/Inventory";
import Status from "@/components/Status";
import Turn from "@/components/Turn";
import Armor from "@/components/Armor";
import Footer from "@/components/Footer";

export default {
  name: 'App',

  components: {
    Footer,
    Armor,
    Turn,
    Status,
    Inventory,
    Header,
    Map,
    Stamina,
    Point
  },

};
</script>

<style scoped>
  .container{
    max-width: 1600px;
  }
</style>
