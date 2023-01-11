<template>
    <div class="nav-background">
  <nav class="nav nav-tabs flex-column">
     <router-link to="/"><img src="../assets/initails.png"></router-link>
     <router-link class="nav-link nav-text-color" to="/">Home</router-link> 
     <router-link class="nav-link nav-text-color" to="/about">About</router-link> 
     <router-link class="nav-link nav-text-color" to="/resume">Resume</router-link> 
     <router-link class="nav-link nav-text-color" to="/projects">Projects</router-link> 
     <router-link class="nav-link nav-text-color" to="/testimonials">Testimonials</router-link> 
     <router-link class="nav-link nav-text-color" to="/contact">Contact Me</router-link>
  </nav>
  </div>
</template>

<script>
    export default {
        name: 'Navbar'
    }
</script>

<style>

.nav-background{
  background: rgba(185, 4, 235, 0.479);
  box-shadow: 0 8px 32px 0 rgba(42, 10, 80, 0.37);
  backdrop-filter: blur(6px);
  -webkit-backdrop-filter: blur(6px);
    display: flex;
  justify-content: center;

}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  overflow: hidden;
  min-height: 100vh;
}


nav img{
  height: 30px;
  width: 60px;
  top: 25px;
  left: 40px;
}

nav {
  width: fit-content;
  height: 65vh;
  border-radius: 20px;
  margin-top: 100px;
  justify-content: space-around;
  text-decoration: none;
  background-color: darkorchid;
  padding: 0 12px !important;
}

nav .nav-text-color{
  width: 100%;
  border-bottom-right-radius: 5px;
 border-bottom-left-radius: 5px;
}

nav .nav-text-color:hover{
  background-color: orchid;
  color: white;
}

nav .nav-link:visited{
  color: white;
}

nav .nav-link:active{
  background-color: orchid;
}

nav .nav-text-color{
  color: white;
}

</style>