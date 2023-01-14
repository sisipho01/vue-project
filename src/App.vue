<template>
  <Navbar/>
  <router-view/>
  <Footer/>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
export default {
  components:{
    Navbar,Footer
  }
}

</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  min-height: 100vh;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color:#1abe59;
}

nav a.router-link-exact-active {
  color: beige;
  text-decoration: none;
}
</style>
