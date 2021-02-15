<template>
  <v-container fluid>
    <v-card
          rounded="xl"
          height="100%"
          width="80%"
          color="rgb(232, 129, 108)"
          class="card-cta"
    >
      <h2>Let's Talk about <br>your project</h2>
      <p>Ready to to take it to the next level? Contact us today and find out how our expertise can help you grow your business</p>
      <!-- <v-btn class="button2" x-large nuxt to="/contact">GET IN TOUCH</v-btn> -->
      <button>Get In Touch</button>
    </v-card>
  </v-container>
</template>

<script>
export default {

}
</script>

<style scoped>
h2{
  color: white;
  text-align: center;
  font-size: 2.1rem;
  font-weight: bold;
  padding: 4%;
  /* letter-spacing: 0.1rem; */
}
p{
  color: white;
  text-align: center;

}

.card-cta{
  margin: 2% 10%;
  padding-bottom: 5rem;
  font-weight: 400;
}

button{
  display: block;
  cursor: pointer;
  background-color: white;
  width: 200px;
  height: 70px;
  border-radius: 30px!important;
  font-size: 1.5rem;
  font-weight: bold;
  color: rgba(248, 99, 0, 0.45);
  box-shadow: 0 0 0 2px  inset;
  margin: 5% 38%;
  /* margin-bottom: 15px; */
}
button:focus {outline:0;}


</style>
