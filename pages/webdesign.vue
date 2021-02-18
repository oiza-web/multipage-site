<template>
<v-container fluid>
  <v-card rounded="xl"
              height="50%"
              width="90%"
              class="card1"
              >
        <v-img height="40vh" src="card1.jpeg">
        <v-card-title> <nuxt-link to='/webdesign' class="title" >WEB DESIGN</nuxt-link> </v-card-title>
        <h4 class="title">we make explicit designs for your ideas, let's help recreate your ideas now!</h4>
        </v-img>
      </v-card>
    <div>
      <div>
        <VueSlickCarousel v-bind="settings">
          <div><img  src="../assets/images/site3.png" height="600px" width="100%" ></div>
          <div><img src="../assets/images/site1.png"  height="600px" width="100%"></div>
          <div><img  src="../assets/images/site3.png" height="600px" width="100%"  ></div>
          <div><img src="../assets/images/site1.png" height="600px" width="100%"></div>
          <!-- <div><img width="90%" src="site2.png" ></div>
          <div><img width="90%" src="site3.png" ></div> -->
        </VueSlickCarousel>
      </div>





    <!-- <Photo v-for="url in photos" :key="url.id"
                                :id ="url.id"
                                :url ="url.url"/> -->
    <!-- <v-card rounded="xl"
              height="40%"
              width="80%"
              class="card2"> -->

        <!-- <v-img height="40vh" v-for="photo in photos" :key="photos.id" >
          {{photos}} -->
          <!-- <v-card-title class="card-text"> APP  DESIGN</v-card-title> -->
        <!-- </v-img> -->
      <!-- </v-card> -->

  <div>
    <v-row>
    <v-col  md="6">
      <v-card rounded="xl"
              height="40%"
              width="80%"
              class="card3">
        <v-img height="40vh" src="card2.jpeg">
          <v-card-title class="card-text" > APP DESIGN</v-card-title>
        </v-img>
      </v-card>
    </v-col>
    <v-col md="6">
      <v-card rounded="xl"
              height="40%"
              width="80%"
              class="card3">

        <v-img  height="40vh" src="card3.jpeg">

        <v-card-title class="card-text1"> GRAPHIC DESIGN</v-card-title>
        </v-img>

      </v-card>
    </v-col>
    </v-row>

  </div>
  <div>
    <call-action></call-action>
    <!-- <footer-section></footer-section> -->
  </div>
  </div>
</v-container>



</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
import axios from 'axios';
import Photo from '../components/Photo';
// import { mapGetters, mapActions} from 'vuex';
export default {

    components: { VueSlickCarousel },
  // components:{
  //   Photo
  // },
  data() {
    return{
      settings: {
          "arrows": false,
          "dots": true,
          "infinite": true,
          "slidesToShow": 1,
          "slidesToScroll": 1,
          "autoplay": true,
          "speed": 2000,
          "autoplaySpeed": 2000,
          "cssEase": "linear"
      },
      // photos : []
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

</script>

<style scoped>
.banner{
  margin: 6% 2%;
  border-radius: 10px;
}
h2{
  color: white;
  text-align: center;
  margin: 10% 5%;
}

p{
  color: white;
  margin-top: 2%;
  font-weight: 600;
  font-size: 1.2em;
}

.card-text{
  color: white;
  margin: 40% 2%;
  text-align: center;
  font-size: 1rem;
  font-weight: 400;
}

.card-text1{
  color: white;
  text-align: center;
  margin: 40% 2%;
  font-size: 1rem;
  font-weight: 400;
}

.card3{
    margin :8% 10%;
    color: white;
}
a{
  text-decoration: none;
  color: white;
}

.card1{
  margin: 8%  5% 2% 5%;
}
.title{
  margin: 5% 2%;
  color: white;

}

</style>
