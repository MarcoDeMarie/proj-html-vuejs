<script>

import Navbar from './partials/header/Navbar.vue'
import Jumbotron from './partials/header/Jumbotron.vue'

export default {
  name: 'Header',
  components:{
      Jumbotron,
      Navbar,
      
  }
}
</script>


<template>

<Navbar />
<Jumbotron />
  

</template>


<style lang="scss" scoped>
@use '../scss/partials/gerneral' as *;
@use '../scss/partials/variables' as *;

</style>