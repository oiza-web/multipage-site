<template>
  <v-col align-self="center">
    <v-row>
      <v-card rounded="xl"
              height="40%"
              width="80%"
              class="card1">

        <v-img height="40vh" src="card1.jpeg">

        <v-card-title class="card-text"> <nuxt-link to='/webdesign' >WEB DESIGN</nuxt-link> </v-card-title>
        </v-img>
      </v-card>
    </v-row>
    <v-row >
      <v-card rounded="xl"
              height="40%"
              width="80%"
              class="card2">

        <v-img height="40vh" src="card2.jpeg">
          <v-card-title class="card-text"> APP  DESIGN</v-card-title>
        </v-img>
      </v-card>
    </v-row>
    <v-row >
      <v-card rounded="xl"
              height="40%"
              width="80%"
              class="card3">

        <v-img  height="40vh" src="card3.jpeg">

        <v-card-title class="card-text1"> GRAPHIC  DESIGN</v-card-title>
        </v-img>

      </v-card>
    </v-row>
  </v-col>
</template>

<script>
export default {

}
</script>

<style scoped>
.card1{
  margin-top: 3rem;
  margin-left: 4rem;
  background-image: 'asset3.jpeg';
}
.card2{
  margin-top: 3rem;
  margin-left: 4rem;
}
.card3{
  margin-top: 3rem;
  margin-left: 4rem;
}

.card-text{
  color: white;
  justify-content: center;
  align-content: center;
}

.card-text1{
  color: white;
  justify-content: center;
  align-content: center;
  font-size: 1.2em;

  /* margin-top: 5.5rem;
  margin-left: 1.3rem; */
  /* font-size: 1.8rem; */
  /* letter-spacing: 0.1rem; */
  /* font-weight: 400; */
}
</style>

