<template>
<div>
  <v-footer class="footer" color="rgb(29, 29, 31)" height="300vh">
    <v-row >
      <v-col cols="4" >
        <nuxt-link to="/"><img src="mpwlogo.png" alt="" height="80px" class="footer-logo"></nuxt-link>
        <p class="footer-logo"> &copy; {{ new Date().getFullYear() }}</p>
      </v-col>

      <v-col cols="4"  class="tcolor"> EDD is Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore eum illo, laborum soluta quasi laudantium doloribus voluptatem quis excepturi laboriosam molestiae qui officia non consequuntur reprehenderit</v-col>
      <v-col cols="4"  class="icon">
        <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-facebook</v-icon></nuxt-link>
        <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-youtube</v-icon></nuxt-link>
        <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-twitter</v-icon></nuxt-link>
        <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-instagram</v-icon></nuxt-link>
      </v-col>
    </v-row>
    <!-- <div class="flex">
      <div>
        <h4 class="spacing"> Our Location</h4>
        <h4 class="spacing">Our Services</h4>
      </div>
    </div>
    <p>Address Lorem ipsum dolor sit, amet  consectetur adipisicing.</p>
    <div class="icons">
      <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-facebook</v-icon></nuxt-link>
      <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-youtube</v-icon></nuxt-link>
      <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-twitter</v-icon></nuxt-link>
      <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-instagram</v-icon></nuxt-link>
    </div> -->
  </v-footer>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>
/* .footer{
  position: unset;
} */
h3{
  color: white;
  font-size: 1em;
  text-align: center;
}
h4{
  color: white;
  font-size: 1em;
  text-align: center;
}
.spacing{

  letter-spacing: 0.09em;
}
.spacing1{

  letter-spacing: 0.09em;
}

p{
  color: white;
  font-weight: bold;
  /* text-align: center; */
}
.icons{
  justify-content: space-around;
}
.flex{
  display: flex;
}
a{
  text-decoration: none;
}

.tcolor{
  color: white;
}
.icon{
  padding: 3%;
}

.footer-logo{
  margin-left: 5%;
}
</style>
