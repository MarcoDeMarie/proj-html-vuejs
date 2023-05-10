<script>
export default {
  name: 'Company'

}
</script>


<template>
  <main>
    <div class="container">
      <p class="watergreen">ABOUT THE NETWORK</p>
      <h1><span>The</span> Company</h1>
      <p class="grey">For 12 years we have been providing audit and warranty, financial andvice, risck advice, taxes and related services to select clients.</p>

      <div class="card-wrapper">
        <div class="card">
          <i class="fa-solid fa-award"></i><h2>Tradition</h2>
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
        </div>
        <div class="card">
          <i class="fa-solid fa-lock"></i><h2>Security</h2>
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
        </div>
        <div class="card">
          <i class="fa-regular fa-pen-to-square"></i><h2>Certificate</h2>
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
        </div>
        <div class="card">
          <i class="fa-solid fa-graduation-cap"></i><h2>Expertise</h2>
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
        </div>
      </div>

      <div class="btn">
        <button class="touch">GET IN TOUCH</button>
        <button class="read">READ MORE</button>
      </div>
    </div>
    <img src="../../../../public/assets/img/about-4.jpg" alt="">

  </main>
  
    
  
  
  
  
</template>


<style lang="scss" scoped>
@use '../../../scss/partials/gerneral' as *;
@use '../../../scss/partials/variables' as *;

main{
  display: flex;
  background-color: #111117;
  height: 880px;
}
.container{
  margin-left: 150px;
  margin-right: 50px;
  
  color: white;
  
}

.card-wrapper{
  display: flex;
  flex-wrap: wrap;
  .card{
    margin-top: 75px;
    margin-right: 30px;
    width: 230px;
    height: 120px;
    h2{
    display: inline;
    font-size: 28px;
    margin-left: 10px;
    }
    i{
    font-size: 25px;
    color: #01a09a;
    }
    p{
      margin-top: 20px;
      color: #95a3af;
      font-size: 18px;
    }
  }
}


h1 {
  margin-top: 30px;
  margin-bottom: 30px;
  font-size: 40px;
  
  span {
    background-color: #0e272d;
    padding: 10px 15px 10px 15px;
    border-radius: 8px;
  }
}

.watergreen{
  margin-top: 130px;
}

.btn{
    display: flex;
    margin-top: 40px;
    .touch{
      border-color: #058283;
      background-color: #058283 ;
      color: white;
      padding: 15px 40px 15px 40px;
      border-radius: 8px;
      font-size: 15px;
      font-weight: bold;
    }
    .read{
      margin-left: 30px;
      background-color: #111117;
      border: 2px solid #058283;
      color: white;
      padding: 15px 40px 15px 40px;
      border-radius: 8px;
      font-weight: bold;
      font-size: 15px;
    }
}

</style>