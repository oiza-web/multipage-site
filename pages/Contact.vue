<template>
  <div>
    <v-container >
      <v-banner  dark shaped outlined class="bg" color="rgb(232, 129, 108)">
      <v-layout row>
        <v-flex  md6 class="color">
          <h1>Contact Us</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Magni eum culpa eius doloremque, accusantium necessitatibus est a
            veniam natus deleniti!</p>
          <v-img src="undraw_Mobile_app_p3ts.svg" height="50%" width="50%" class="size"></v-img>

        </v-flex>
        <v-flex xs12 md6 class="color">
        <v-form
        class="form"

        lazy-validation
      >
        <p>Send us a message, Kindly fill the form below</p>
        <v-text-field
          class="size"
          solo
          color="white"
          rounded
          label="Name"
          required
          type="text"
        ></v-text-field>
        <v-select
          class="size"
          solo
          color="white"
          rounded
          label="How did you hear about us?"
          v-model="values"
          :items = "items"
        >

        </v-select>

        <v-text-field
          class="size"
          label="E-mail"
          type="email"
          required
          solo
          rounded
          color="white"
        ></v-text-field>

        <v-textarea
          class="size"
          rounded
          solo
          color="white"
          name="input-7-1"
          label="Message"
          value="Hi, I would love to build a mobile application, How much would it cost?"
          hint="Hint text"
        ></v-textarea>

        <v-btn class="btn" rounded>
          Submit
        </v-btn>

    </v-form>
        </v-flex>
      </v-layout>
</v-banner>
    </v-container>

<v-container  fluid class="avatar">
  <v-layout row>
  <v-flex xs12 md4>
    <v-avatar size="100"  class="mt">
    <v-img src="undraw_Mobile_app_p3ts.svg"></v-img>
    </v-avatar>
    <h5>NETHELANDS</h5>
    <v-btn rounded class="button" color="rgb(232, 129, 108)"  nuxt>LOCATION</v-btn>
  </v-flex>
  <v-flex xs12 md4>
    <v-avatar size="100"  class="mt">
      <v-img src="undraw_Mobile_app_p3ts.svg"></v-img>
    </v-avatar>
    <h5>CANADA</h5>
    <v-btn class="button" rounded color="rgb(232, 129, 108)"  nuxt>LOCATION</v-btn>
  </v-flex>
  <v-flex xs12 md4>
    <v-avatar size="100"  class="mt">
      <v-img src="undraw_Mobile_app_p3ts.svg"></v-img>
    </v-avatar>
    <h5>NIGERIA</h5>
  <v-btn class="button" rounded color="rgb(232, 129, 108)"  nuxt>LOCATION</v-btn>
  </v-flex>
  </v-layout>
</v-container>
    <call-action></call-action>
  </div>


</template>

<script>
export default {
    data: () => ({
      items: ['foo', 'bar', 'fizz', 'buzz'],
    }),
  }
</script>

<style scoped>
.btn{
  margin: 3% 8%;
}
.size{
  max-width: 80%;
  margin: 0 8%;
}
.bg{
  margin-top: 10%;
}
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
/* background-color: rgb(232, 129, 108); */
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
.form{
  margin-left: 4%;
}

.mt{
  margin-top: 3em;
}
</style>
