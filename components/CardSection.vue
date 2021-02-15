<template>
<v-container fluid>
  <v-layout row>
  <v-flex xs12 md4 d-flex flex-column lg-6  >
  <v-card rounded="xl"
              height="40%"
              width="80%"
              class="card1"
              >
        <v-img height="40vh" src="card1.jpeg">
        <v-card-title class="card-text"> <nuxt-link to='/webdesign' >WEB DESIGN</nuxt-link> </v-card-title>
        </v-img>
      </v-card>
  </v-flex>
  <v-flex xs12 md4 d-flex flex-row lg-3 d-flex-wrap>
  <v-card rounded="xl"
              height="40%"
              width="80%"
              class="card2">

        <v-img height="40vh" src="card2.jpeg">
          <v-card-title class="card-text"> APP  DESIGN</v-card-title>
        </v-img>
      </v-card>
  </v-flex>
  <v-flex xs12 md4 d-flex flex-row lg-3 flex-wrap>
  <v-card rounded="xl"
              height="40%"
              width="80%"
              class="card3">

        <v-img  height="40vh" src="card3.jpeg">

        <v-card-title class="card-text1"> GRAPHIC  DESIGN</v-card-title>
        </v-img>

      </v-card>
  </v-flex>
  </v-layout>
</v-container>


</template>

<script>
export default {

}
</script>

<style scoped>
.card1{
  margin :5% 10%;
  background-image: 'asset3.jpeg';
}
.card2{
    margin :5% 10%;
}
.card3{
    margin :5% 10%;
}

.card-text{
  color: white;
  justify-content: center;
  align-content: center;
  font-size: 1em;
}

.card-text1{
  color: white;
  justify-content: center;
  align-content: center;
  font-size: 1em;
}

a{
  text-decoration: none;
  color: white;
}
</style>

