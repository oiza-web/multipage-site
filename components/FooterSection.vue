<template>
<div>
  <v-footer class="footer" color="rgb(29, 29, 31)" height="1000%">
    <div>
      <h3>THEBRANDNAME</h3>
    <h4 class="spacing1">OUR COMPANY</h4>
    <h4 class="spacing"> OUR LOCATION</h4>
    <h4 class="spacing">OUR SERVICES</h4>
    <p>Address</p>
    <p>Lorem ipsum dolor sit, amet <br> consectetur adipisicing.</p>
    <p>Address</p>
    <p>Lorem ipsum dolor sit, amet <br> consectetur adipisicing.</p>
    <div class="icons">
      <v-icon color="rgb(232, 129, 108)">mdi-facebook</v-icon>
      <v-icon color="rgb(232, 129, 108)">mdi-youtube</v-icon>
      <v-icon color="rgb(232, 129, 108)">mdi-twitter</v-icon>
      <v-icon color="rgb(232, 129, 108)">mdi-pinterest</v-icon>
      <v-icon color="rgb(232, 129, 108)">mdi-instagram</v-icon>

    </div>
    </div>






  </v-footer>
</div>



</template>

<script>
export default {

}
</script>

<style scoped>
.footer{
  position: unset;
}
h3{
  color: white;
  font-size: 1.5em;
  margin-left: 5em;
  margin-top: 8em;

}
h4{
  color: white;
  font-size: 1.5em;
  margin-left: 5em;
  font-weight: 350;
}
.spacing{
  margin-top: 2em;
  letter-spacing: 0.09em;
}
.spacing1{
  margin-top: 3em;
  letter-spacing: 0.09em;
}

p{
  color: white;
  margin-top: 2em;
  margin-left: 7em;
}
.icons{
  margin-left: 7em;
  justify-content: space-around;
}
</style>
