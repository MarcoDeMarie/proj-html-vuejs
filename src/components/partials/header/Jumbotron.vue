<script>
export default {
  name: 'Jumbotron'

}
</script>


<template>
  <header>
    <div class="navbar container">
      <div class="logo">
        <img src="/assets/img/logo.PNG" alt="">
      </div>
      <ul>
        <li>HOME</li>
        <li>SERVICES</li>
        <li>ABOUT</li>
        <li>PROJECTS</li>
        <li>RESULTS</li>
        <li><span>GET IN TOUCH</span></li>
      </ul>
    </div>

    <div class="ready-team">
      <h1>Ready <span>Team</span></h1>
      <p>no matte what your company needs, we will be ready to assist you in the best possible way</p>
      <div class="btn">
        <button class="touch">GET IN TOUCH</button>
        <button class="read">READ MORE</button>
      </div>
    </div>


    <img src="/assets/img/bg-parallax-2.png" alt="">
  </header>
  
</template>


<style lang="scss" scoped>
@use '../../../scss/partials/gerneral' as *;
@use '../../../scss/partials/variables' as *;

header{
  height: 770px;
  img{
    object-fit: cover ;
  }
}

.ready-team{
  position: absolute;
  display: flex;
  flex-direction: column;
  width: 500px;
  height: 300px;
  text-align: center;
  left: 600px;
  top: 400px;
  h1{
    font-weight: bold;
    font-size: 80px;
    span{
      background-color: #d5e7e8;
      color: #058283;
      padding: 10px 15px 10px 15px ;
      border-radius: 8px;
    }
  }
  p{
    margin-top: 30px;
    font-size: 25px;
    color:#606d75 ;
  }
  .btn{
    display: flex;
    justify-content: center;
    margin-top: 30px;
    .touch{
      background-color: #058283 ;
      color: white;
      padding: 15px 40px 15px 40px;
      border-radius: 8px;
      font-size: 15px;
      font-weight: bold;
    }
    .read{
      margin-left: 30px;
      background-color: white;
      border: 2px solid #058283;
      color: #058283;
      padding: 15px 40px 15px 40px;
      border-radius: 8px;
      font-weight: bold;
      font-size: 15px;
    }
  }
}

.navbar{
  margin-top: 15px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.logo{
  height: 45px;
  width: 170px;
}

ul{
  list-style: none;
  display: flex;
  li{
    margin-right: 40px;
    color: #606d75;
    font-weight:  bold ;
    span{
      background-color: #058283 ;
      color: white;
      padding: 15px 40px 15px 40px;
      border-radius: 8px;
    }
  }
}



</style>