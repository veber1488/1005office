<template>
  <div class="app-container documentation-container">
 <v-app id="inspire">
   <v-card style="background-color: #34495e; color: #bdc3c7;"><h1 class="display-1">Net Offline Configuration: <strong>Actions</strong></h1><h3 class="headline">To select the desired action, press the button below</h3></v-card>
   
    <v-layout row justify-center>
      <v-btn color="primary" dark large @click.native.stop="dialog = true" style="width: 200px;" class="headline">Actions</v-btn>
    
      <v-dialog v-model="dialog" max-width="1500">
       
        <v-container fluid grid-list-md style="color: black;">
      <v-layout row wrap>
        <v-flex d-flex xs12 sm6 md2 style="color: black;">
          <router-link to="/net_off_config/addDevice">
          <v-card color="grey lighten-2" dark class="grow">
            <v-card-title primary class="title" style="color: black;">Add Devices</v-card-title>
            <hr>
            <v-card-text style="color: black;">{{ lorem }}</v-card-text>
          </v-card></router-link>
        </v-flex>
        <v-flex d-flex xs12 sm6 md2>
          <v-card color="grey lighten-2" dark class="grow">
            <v-card-title primary class="title" style="color: black;">Add Modules</v-card-title>
            <hr>
            <v-card-text>lorem</v-card-text>
          </v-card>
        </v-flex>
        <v-flex d-flex xs12 sm6 md2>
          <v-card color="grey lighten-2" dark class="grow">
            <v-card-title primary class="title" style="color: black;">Add Cables</v-card-title>
            <hr>
            <v-card-text>{{ lorem }}</v-card-text>
          </v-card>
        </v-flex>
        <v-flex d-flex xs12 sm6 md2>
          <v-card color="grey lighten-2" dark class="grow">
            <v-card-title primary class="title" style="color: black;">Add Ports, VPNs, etc</v-card-title>
            <hr>
            <v-card-text>{{ lorem }}</v-card-text>
          </v-card>
        </v-flex>
        <v-flex d-flex xs12 sm6 md2>
          <router-link to="/dashboard">
          <v-card color="grey lighten-2" dark class="grow">
            <v-card-title primary class="title" style="color: black;">Add E1 Ring</v-card-title>
            <hr>
            <v-card-text>{{ lorem }}</v-card-text>
          </v-card></router-link>
        </v-flex>
        <v-flex d-flex xs12 sm6 md2>
          <v-card color="grey lighten-2" dark class="grow">
            <v-card-title primary class="title" style="color: black;">Empty</v-card-title>
            <hr>
            <v-card-text>{{ lorem }}</v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
      </v-dialog>
    </v-layout>
  </v-app>
  </div>
</template>
<script>
import DropdownMenu from '@/components/Share/dropdownMenu'

export default {
  name: 'documentation1',
  components: { DropdownMenu },
  data() {
    return {
      dialog: false,
      lorem: `Lorem ipsum dolor sit amet, mel at clita quando. Te sit oratio vituperatoribus, nam ad ipsum posidonium mediocritatem, explicari dissentiunt cu mea. Repudiare disputationi vim in, mollis iriure nec cu, alienum argumentum ius ad. Pri eu justo aeque torquatos.`
    }
  }
}
</script>

<style rel="stylesheet/scss" lang="scss" scoped>

@import url('https://fonts.googleapis.com/css?family=Roboto');

.documentation-container {
  margin: 0px;
  .document-btn {
    float: left;
    margin-left: 50px;
    vertical-align: middle;
    display: block;
    cursor: pointer;
    background: black;
    color: white;
    height: 60px;
    width: 200px;
    line-height: 60px;
    font-size: 20px;
    text-align: center;
  }
}
.grow { transition: all .3s ease-in-out; }
.grow:hover { transform: scale(1.05); }



</style>
