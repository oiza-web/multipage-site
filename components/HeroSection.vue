<template>
  <v-banner color="rgb(232, 129, 108)"
  height="40%" outlined >
  <h2>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</h2>
  <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Cupiditate alias libero quia dolore, a quasi! Impedit ipsa odio sit quae alias explicabo tempora itaque quas?</p>
  <v-btn class="button" x-large elevation="0" to="/about" nuxt>Learn more</v-btn>
  <div>
    <v-img src="asset2.jpeg" class="image">

  </v-img>
  </div>


  </v-banner>
</template>

<script>
export default {

}
</script>

<style scoped>
p{
  color: white;
  text-align: center;
  margin-top: 4rem;
}

h2{
  color: white;
  text-align: center;
  margin-top: 4rem;
  line-height: 2.5rem;
  font-size: 2.5rem;
  font-weight: 400;
}

.button{
  /* align-content: center; */
  margin-left: 10rem;
  margin-top: 3rem;
  padding: 4rem;
}

.image{
  margin-top:7rem;
  border-top-left-radius: 2rem;
  border-top-right-radius: 2rem;
  height: 70%;
}
</style>>

