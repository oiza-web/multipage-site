<template>
  <v-container fluid>
    <v-layout row>
        <v-flex xs12 md6 class="color">
          <h1>About Us</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni eum culpa eius doloremque, accusantium necessitatibus est a veniam natus deleniti!</p>
        </v-flex>
        <v-flex xs12 md6>
          <v-img src="asset1.jpeg"></v-img>
        </v-flex>
      </v-layout>


      <v-layout row>
        <v-flex xs12 md6 >
        <v-img src="femaledeveloper.jpeg"></v-img>
        </v-flex>
        <v-flex xs12 md6 class="color2">
          <h1 class="color3">About Us</h1>
          <p class="color4"> Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni eum cul</p>
        </v-flex>
      </v-layout>

<v-container fluid class="avatar">
  <v-layout row>
  <v-flex xs12 md4>
    <v-avatar size="100"  class="mt">
    <v-img src="undraw_Mobile_app_p3ts.svg"></v-img>
    </v-avatar>
    <h5>NETHELANDS</h5>
    <v-btn class="button" color="rgb(232, 129, 108)" to="/Location" nuxt>LOCATION</v-btn>
  </v-flex>
  <v-flex xs12 md4>
    <v-avatar size="100"  class="mt">
      <v-img src="undraw_Mobile_app_p3ts.svg"></v-img>
    </v-avatar>
    <h5>CANADA</h5>
    <v-btn class="button" color="rgb(232, 129, 108)" to="/Location" nuxt>LOCATION</v-btn>
  </v-flex>
  <v-flex xs12 md4>
    <v-avatar size="100"  class="mt">
      <v-img src="undraw_Mobile_app_p3ts.svg"></v-img>
    </v-avatar>
    <h5>NIGERIA</h5>
  <v-btn class="button" color="rgb(232, 129, 108)" to="/Location" nuxt>LOCATION</v-btn>
  </v-flex>
  </v-layout>
</v-container>
            <call-action></call-action>
  </v-container>





</template>

<script>
export default {

}
</script>

<style scoped>
h1{
  color: white;
  margin-left: 5rem;
  margin-top: 6rem;
}
p{
  color: white;
  margin-left: 5rem;
  margin-top: 6rem;
  margin-right: 3rem;
  margin-bottom: 2rem;
}

.color{
background-color: rgb(232, 129, 108);
width: 50;
height: 500;
}

.color2{
  background-color: rgb(253, 244, 241);
}

.color3{
  color: rgb(232, 129, 108);
}

.color4{
  color: black;
}

.avatar{
  margin: 5em 2em 5em 10em;
}

h5{
  margin-top: 2em;
  font-weight: lighter;
}

.button{
  margin-top: 2em;

}

.mt{
  margin-top: 3em;
}
</style>
