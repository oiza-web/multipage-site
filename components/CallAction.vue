<template>
  <div>
    <v-card
          rounded="xl"
          height="100%"
          width="80%"
          color="rgb(232, 129, 108)"
          class="card-cta"

    >
      <h2>Let's Talk about <br>your project</h2>
      <p>Ready to to take it to the next level? Contact us today and find out how our expertise can help you grow your business</p>
      <v-btn class="button2" x-large nuxt to="/contact">GET IN TOUCH</v-btn>
    </v-card>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
h2{
  color: white;
  margin-left: 5rem;
  padding-top: 6rem;
  font-size: 2.1rem;
  font-weight: 450;
  /* letter-spacing: 0.1rem; */
}
p{
  color: white;
  margin-top: 1.8rem;
  margin-left: 1.8rem;
  margin-right: 1.8rem;


}

.card-cta{
  margin-top: 8rem;
  margin-left: 3rem;

  padding-bottom: 5rem;
  /* position: relative; */
  z-index: -0.5;
  position: unset;



}
.button2{
  margin-left: 8rem;
  margin-top: 3rem;

}
</style>
