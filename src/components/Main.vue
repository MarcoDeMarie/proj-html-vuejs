<script>
import Services from './partials/main/Services.vue'
import Company from './partials/main/Company.vue'
import Project from './partials/main/Project.vue'
import Results from './partials/main/Results.vue'

export default {
  name: 'Main',
  components:{
      Services,
      Company,
      Project,
      Results
  }

}
</script>


<template>

<Services />

<Company />

<Project />

<Results />
  
  
</template>


<style lang="scss" scoped>
@use '../scss/partials/gerneral' as *;
@use '../scss/partials/variables' as *;

</style>