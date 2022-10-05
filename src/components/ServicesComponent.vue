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
    <div class="services-bottom"></div>
  </div>
</template>

<script>
export default {
  name: "ServicesComponent",
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

    p {
      color: #be9359;
      font-family: Helvetica, Arial;
      font-size: 1.05rem;
      font-weight: bold;
      letter-spacing: 1.8px;
    }

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
}
</style>