<template>
<nav class="navbar">
  <div class="brand-title" v-if="mobileView" @click="toggle = !toggle">
    <nuxt-link to="/" tag="div"><v-img height="8vh" width="10vh" src="logo.png"></v-img></nuxt-link>

  </div>
        <a href="#" class="toggle">
        <span class="bar"></span>
        <span class="bar"></span>
        <span class="bar"></span>
        </a>
        <div class="navbar-links">
        <ul>
            <li> <nuxt-link to="/Company"> Our Company</nuxt-link></li>
            <li><nuxt-link to="/Location">Locations</nuxt-link></li>
            <li><nuxt-link to="/Contact"> Contact</nuxt-link></li>
            <!-- <li><nuxt-link to="/Services"> Services</nuxt-link></li> -->

        </ul>
        </div>
</nav>
</template>

<script>
export default{
  data(){
    return{
      toggle: false,
      mobileView: true
    }
  }
}
</script>

<style scoped>



body {
    margin: 0;
    padding: 0;
}

.navbar {
    margin-top: 2rem;
    padding-bottom: 1em;
    display: flex;
    position: relative;
    justify-content: space-between;
    align-items: center;
    background-color: white;
    color: black;
}

.brand-title {
    font-size: 1.5rem;
    /* margin: .1rem; */
    font-weight: bold;
    color: rgb(29, 29, 31);
}

.navbar-links {
    height: 100%;
}

.navbar-links ul {
    display: flex;
    margin: 0;
    padding: 0;
}

.navbar-links li {
    list-style: none;
}

.navbar-links li a {
    display: block;
    text-decoration: none;
    color: black;
    padding: 1rem;
}

.navbar-links li:hover {
    background-color: rgb(232, 129, 108);
}

.toggle {
    position: absolute;
    top: .75rem;
    right: 1rem;
    display: none;
    flex-direction: column;
    justify-content: space-between;
    width: 30px;
    height: 21px;
}

.toggle .bar {
    height: 3px;
    width: 100%;
    background-color: black;
    border-radius: 10px;
}

@media (max-width: 800px) {
    .navbar {
        flex-direction: column;
        align-items: flex-start;
    }

    .toggle{
        display: flex;
    }

    .navbar-links {
        display: none;
        width: 100%;
    }

    .navbar-links ul {
        width: 100%;
        flex-direction: column;
    }

    .navbar-links ul li {
        text-align: center;
    }

    .navbar-links ul li a {
        padding: .5rem 1rem;
    }

    .navbar-links.active {
        display: flex;
    }
}
</style>
