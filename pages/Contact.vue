<template>
  <div>
    <v-container fluid>
      <v-layout row>
        <v-flex xs12 md6 class="color">
          <h1>Contact Us</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni eum culpa eius doloremque, accusantium necessitatibus est a veniam natus deleniti!</p>
        </v-flex>
        <v-flex xs12 md6 class="color">
          <v-form
        ref="form"
        v-model="valid"
        lazy-validation
      >
        <v-text-field
          v-model="name"

          :rules="nameRules"
          label="Name"
          required
        ></v-text-field>

        <v-text-field

          v-model="email"
          :rules="emailRules"
          label="E-mail"
          required
        ></v-text-field>


        <v-text-field
          v-model="email"
          :rules="emailRules"
          label="E-mail"
          required
        ></v-text-field>


        <v-text-field
          v-model="email"
          :rules="emailRules"
          label="E-mail"
          required
        ></v-text-field>



        <v-checkbox

          v-model="checkbox"
          :rules="[v => !!v || 'You must agree to continue!']"
          label="Do you agree?"
          required
        ></v-checkbox>

        <v-btn class="button">
          Submit
        </v-btn>

    </v-form>
        </v-flex>
      </v-layout>
</v-container>
<v-container class="avatar">
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
  </div>


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
  margin-bottom: 2em;

}

.mt{
  margin-top: 3em;
}
</style>
