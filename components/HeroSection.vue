<template>
<v-container fluid class="background">
  <div >
  <div>
    <h1>Welcome to EDD technologies</h1>
    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officia harum quibusdam, asperiores hic labore dolorem optio rerum fugit beatae maxime.</p>
  </div>

  <div>
    <nuxt-link to="/contact"><button>Learn More</button></nuxt-link>
  </div>
</div>
</v-container>
</template>

<script>
export default {

}
</script>

<style scoped>
p{
  color: white;
  text-align: center;
  padding-bottom: 20%;
  font-weight: bold;
  font-size: 1.2em;
}

h1{
  color: white;
  text-align: center;
  padding: 70px 0;
  font-size: 2.5rem;

}

.background{

  background:
    linear-gradient(
      rgb(232, 129, 108),
      rgba(248, 99, 0, 0.45)
    ),
    url('../static/asset2.jpeg');
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
      background-size: cover;
      min-height: 90vh;

}

button{
  display: block;
  cursor: pointer;
  outline: none;
  border: none;
  background-color: white;
  width: 200px;
  height: 70px;
  border-radius: 50px;
  font-size: 1.5rem;
  font-weight: 600;
  color: rgba(248, 99, 0, 0.45);
  background-size: 100% 100%;
  box-shadow: 0 0 0 2px  inset;
  margin: 0 25%;
}

a{
  text-decoration: none;
}

@media (min-width: 600px) {
  button {
    margin: 0 35%;
  }
  .background{
    padding-top: 5%;
  }
}

@media (min-width: 940px) {
  button {
    margin: 0 40%;

  }
  p{
    font-size: 2em;
    font-weight: 100;
    letter-spacing: .0002em;
  }
  h1{
    font-size: 3em;
  }
}
</style>

