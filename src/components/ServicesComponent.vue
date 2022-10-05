<template>
  <div id="services-container">
    <div class="services-top">
      <div class="triangle-div"></div>

      <div class="award-zone">
        <p>AWARD WINNING</p>
        <h2>Pro Barbers</h2>
        <button>MEET YOUR NEW BARBER</button>
      </div>
    </div>

    <div class="services-bottom">
      <div class="triangle-div"></div>

      <div class="services-zone">
        <p>MENS GROOMING</p>
        <h2>Services</h2>
        <div>
          <div v-for="service in services" :key="service.name">
            <div>
              <img
                :src="require(`../assets/img/${service.image}`)"
                :alt="service.name"
              />
            </div>
            <h3>
              {{ service.name }}
            </h3>
            <span>
              {{ service.description }}
            </span>
          </div>
        </div>
      </div>
      <div id="bottom-button">
        <button>READ ABOUT OUR SERVICES</button>
      </div>
    </div>
  </div>
</template>

<script>
import { services } from "@/data.js";

export default {
  name: "ServicesComponent",

  data() {
    return {
      services: services,
    };
  },
};
</script>

<style lang="scss" scoped>
.services-top {
  position: relative;
  min-height: 556px;
  background-image: url("../assets/img/avadabarbers-about-introbackground.jpg");
  background-size: cover;
  margin: 0 auto;

  .award-zone {
    padding-top: 140px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    h2 {
      font-family: "Abril", Helvetica, Arial;
      font-size: 3.95rem;
      letter-spacing: 4px;
      color: #b1b1b1;
    }

    button {
      margin-top: 30px;
      width: 300px;
      padding: 18px 20px;
      font-size: 1.1rem;
      background-color: rgba(0, 0, 0, 0);
      color: #be9359;
      border: 2px solid #be9359;
    }
  }
}

.services-bottom {
  position: relative;
  min-height: 1000px;
  background-color: white;
  margin: 0 auto;

  .triangle-div {
    border-bottom: 100px solid #121314 !important;
  }

  .services-zone {
    padding-top: 100px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    h2 {
      font-family: "Abril", Helvetica, Arial;
      font-weight: 100;
      font-size: 4.4rem;
      letter-spacing: 2px;
      color: #b1b1b1;
      margin-top: 5px;
      margin-bottom: 80px;
    }

    img {
      width: 65px;
      height: 110px;
    }
  }

  #bottom-button {
    text-align: center;
    margin-top: 300px;

    button {
      width: 300px;
      padding: 18px 20px;
      font-size: 1.1rem;
      background-color: rgba(0, 0, 0, 0);
      color: #be9359;
      border: 2px solid #be9359;
    }
  }
}

// area where services with their images are displayed
.services-zone > div {
  display: flex;
  justify-content: center;
  align-items: center;
  column-gap: 100px;

  div {
    width: 300px;
    height: 150px;
    text-align: center;
  }

  h3 {
    margin-bottom: 50px;
    height: 45px;
    color: #be9359;
    font-family: "Abril", Helvetica, Arial;
    font-size: 2rem;
    font-weight: 100;
  }

  span {
    color: #686868;
    font-family: Helvetica, Arial;
    font-size: 1.1rem;
    line-height: 2rem;
  }
}

p {
  color: #be9359;
  font-family: Helvetica, Arial;
  font-size: 1.05rem;
  font-weight: bold;
  letter-spacing: 1.8px;
}

// this is the triangle shaped div that separes some sections
.triangle-div {
  position: absolute;
  bottom: 0;
  height: 0;
  left: 0;
  width: 0px;
  border-left: 950px solid transparent;
  border-right: 950px solid transparent;
  border-bottom: 100px solid white;
}

.services-zone div div:nth-child(2) img {
  width: 85px;
}
</style>