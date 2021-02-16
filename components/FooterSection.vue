<template>

<v-container fluid class="footer">
  <v-row align-content="space-around" >
    <v-col cols="12" md="4" >
        <nuxt-link to="/"><img src="mpwlogo.png" alt="" height="80px" class="footer-logo"></nuxt-link>
        <h4 class="footer-logo"> </h4>
    </v-col>

    <v-col cols="12" md="4" >
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Unde delectus quisquam quo iste? At, fuga. </p>

    </v-col>
    <v-col cols="12"  md="4" >
        <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-facebook</v-icon></nuxt-link>
        <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-youtube</v-icon></nuxt-link>
        <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-twitter</v-icon></nuxt-link>
        <nuxt-link to="/"><v-icon color="rgb(232, 129, 108)">mdi-instagram</v-icon></nuxt-link>
        <p>&copy; {{ new Date().getFullYear() }}</p>
    </v-col>

  </v-row>
</v-container>
</template>

<script>
export default {

}
</script>

<style scoped>

.footer{
  background-color: black;
  height: 50%;
  color: white;
}
a{
  text-decoration: none;
}
p{
  font-weight: bold;
}
h2{
  margin-right: 10%;
}
/* .footer{
  position: unset;
} */
/* h3{
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
} */

/* p{
  color: white;
  font-weight: bold;

} */
/* .icons{
  justify-content: space-around;
}
.flex{
  display: flex;
}


.tcolor{
  color: white;
}
.icon{
  padding: 3%;
} */

/* .footer-logo{
  margin-left: 5%;
} */
</style>
