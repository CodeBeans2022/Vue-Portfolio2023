<template>
  <div class="gridContainer">
    <router-view/>
    <Navbar/>
</div>
<Footer class="container-fluid text-light text-center position-fixed bottom-0"
    style="height: 50px; width: 87.5%; padding: 10px; z-index:10; background-color:darkorchid;">Jamie-Lee Kinnear 2022</Footer>
</template>

<script>

import Navbar from '@/components/Navbar.vue'

export default {
  components: {
    Navbar
  }
}
</script>

<style>

.gridContainer{
  display: grid;
  grid-template-columns: 7fr 1fr;
  grid-template-rows: 1fr;
  min-height: 100vh;

}

@media screen and (max-width: 760px){
  .gridContainer{
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr;
  }

  .nav-background{
    display: none !important;
  }
  .navMobile{
    display: block !important;
  }
}

*{
  text-decoration: none;
}

@media screen and (max-width: 760px){
  Footer{
    width: 100% !important;
  }
}

</style>
