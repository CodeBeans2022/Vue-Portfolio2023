<template>
  <div class="gridContainer">
    <router-view/>
    <Navbar/>
</div>
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

</style>
