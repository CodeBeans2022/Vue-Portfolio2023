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

}

</style>
