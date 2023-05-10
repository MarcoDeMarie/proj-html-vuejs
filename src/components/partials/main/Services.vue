<script>

import { Services } from '../../../data/Service';

export default {
  name: "Services",

  data() {
      return {
        Services
      }
    }
};
</script>


<template>
  <main>
    <div class="container">
      <p class="watergreen">OUR BUSINESS AREAS</p>
      <h1>Excellence in <span>Services</span></h1>
      <div class="d-flex">
        <p>
          We are leaders in providin consultancy services with a set of
          cutting-edge technologies and a tem of experineces and renowned
          professionals. These are some options that you can hire.
        </p>
        <button>SEE ALL</button>
      </div>

      <div class="card-wrapper">
        <div v-for="(service, index) in Services"
        :key="index"
        class="card">
          <img :src="service.Image" alt="" />
          <i class="fa-solid fa-arrow-right"></i>
          <div class="text">
            <h2>{{ service.title }}</h2>
            <p>{{ service.text }}</p>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>


<style lang="scss" scoped>
@use "../../../scss/partials/gerneral" as *;
@use "../../../scss/partials/variables" as *;

main {
  background-color: #eef4ed;
}

.container{
  padding-top: 130px;
  padding-bottom: 160px;
}

.d-flex {
  display: flex;
  justify-content: space-between;
  margin-top: 30px;
  p {
    color: #606d75;
  }
}

h1 {
  font-size: 40px;
  span {
    background-color: #d5e7e8;
    color: #058283;
    padding: 10px 15px 10px 15px;
    border-radius: 8px;
  }
}

button {
  margin-left: 200px;
  width: 180px;
  background-color: #058283;
  color: white;
  padding: 15px 40px 15px 40px;
  border-radius: 8px;
  font-size: 19px;
}
.watergreen {
  color: #12a6a7;
  font-weight: bold;
}

.card-wrapper {
  display: flex;
  flex-wrap: wrap;
  margin-top: 60px;
  .card {
    background-color: #ffffff;
    height: 260px;
    width: 350px;
    margin-bottom: 30px;
    margin-right: 30px;
    border-radius: 8px;
    i {
      position: relative;
      bottom: 60px;
      left: 190px;
      font-size: 30px;
      color: #82c1c1;
    }

    img {
      margin: 45px 0 30px 45px;
      height: 50px;
      width: 50px;
    }

    .text {
      margin: 0 85px 0 45px;

      h2 {
        font-size: 26px;
      }
      p {
        color: #606d75;
        font-size: 18px;
        margin-top: 15px;
        margin-bottom: 60px;
      }
    }
  }
}
</style>