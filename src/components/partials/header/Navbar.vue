<script>
export default {
  name: 'Navbar'

}
</script>


<template>
  <header>

    <div class="info-bar container">
      <div class="orari">
        <p><i class="fa-solid fa-clock"></i>Open Hours: Mon - Sat - 9:00 - 18:00</p>
      </div>

      <div class="contatti">

        <p><i class="fa-solid fa-phone"></i>+1 (305) 1234-5678</p>
        <p><i class="fa-solid fa-envelope"></i>hello@example.com</p>

        <div class="icons">
          <i class="fa-brands fa-facebook-f"></i>
          <i class="fa-brands fa-twitter"></i>
          <i class="fa-brands fa-linkedin-in"></i>
        </div>
      </div>
    </div>

  </header>

  
  
  
</template>


<style lang="scss" scoped>
@use '../../../scss/partials/gerneral' as *;
@use '../../../scss/partials/variables' as *;

header{
  background-color: #21333e ;
  color: #e2e3e7;
}
.info-bar{
  display: flex;
  justify-content: space-between;
  padding-top: 15px;
  height: 50px;
}
i{
  margin-right: 10px;
}
.contatti{
  display: flex;
  p{
  margin-left: 35px;
  }
}

.icons{
  i{
    margin-left: 30px;
  }
}
</style>