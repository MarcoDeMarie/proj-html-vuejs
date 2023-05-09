<script>

import Infobar from './partials/header/Infobar.vue'
import Jumbotron from './partials/header/Jumbotron.vue'

export default {
  name: 'Header',
  components:{
      Jumbotron,
      Infobar,
      
  }
}
</script>


<template>

<Infobar />
<Jumbotron />
  

</template>


<style lang="scss" scoped>
@use '../scss/partials/gerneral' as *;
@use '../scss/partials/variables' as *;

</style>