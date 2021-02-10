<template>
  <div>
  <v-banner color="rgb(232, 129, 108)" height="300" outlined >
    <h2>Web Design</h2>
    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Cupiditate alias libero quia dolore, a quasi! Impedit ipsa odio sit quae alias explicabo tempora itaque quas?</p>
  </v-banner>
  <div>

    <Photo v-for="url in photos" :key="url.id"
                                :id ="url.id"
                                :url ="url.url"/>
    <!-- <v-card rounded="xl"
              height="40%"
              width="80%"
              class="card2"> -->

        <!-- <v-img height="40vh" v-for="photo in photos" :key="photos.id" >
          {{photos}} -->
          <!-- <v-card-title class="card-text"> APP  DESIGN</v-card-title> -->
        <!-- </v-img> -->
      <!-- </v-card> -->
  </div>
  <div>
    <v-col>
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

        <v-card-title class="card-text1"> GRAPHIC DESIGN</v-card-title>
        </v-img>

      </v-card>
    </v-row>
    </v-col>

  </div>
  <div>
    <call-action></call-action>
    <footer-section></footer-section>
  </div>
  </div>


</template>

<script>
import axios from 'axios';
import Photo from '../components/Photo';
// import { mapGetters, mapActions} from 'vuex';
export default {
  components:{
    Photo
  },
  data(){
    return{
      photos : []
    }
  },
  async created(){
    const config = {
      headers:{
        'Accept' :'application/json'
      }
    }

    try {
      const res = await axios.get('https://jsonplaceholder.typicode.com/photos?_limit=4', config)
      console.log(res.data)
      this.photos = res.data
    }
    catch{
      console.log(err)
    }

  }

  }
  // computed: mapGetters(['allImages']),
  // methods:{
  //   ...mapActions(['fetchImages']),
  //   fetchImages(){
  //     this.fetchImages();
  //   }
</script>

<style scoped>
h2{
  color: white;
}

p{
  color: white;
  margin-top: 3rem;
}

.card-text{
  color: white;
  margin-top: 5.5rem;
  margin-left: 3em;
  font-size: 1.5rem;
  letter-spacing: 0.1rem;
  font-weight: 400;
}

.card-text1{
  color: white;
  margin-top: 5.5rem;
  margin-left: 1.3rem;
  font-size: 1.8rem;
  letter-spacing: 0.1rem;
  font-weight: 400;
}

.card2{
  margin-top: 3rem;
  margin-left: 4rem;
}
.card3{
  margin-top: 3rem;
  margin-left: 4rem;
}
</style>
