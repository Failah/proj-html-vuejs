<template>
  <div>
    <div id="top-half-footer">
      <div>
        <div>
          <img
            class="resize-img"
            src="../assets/img/avadabarbers_footer_shop_image.png"
            alt="Footer Shop"
          />
        </div>
        <button>SHOP OUR RANGE NOW</button>
      </div>
      <div>
        <div>
          <img src="../assets/img/avadabarbers-logo-x1.png" alt="Avada Logo" />
        </div>
        <div class="agency-infos">
          <div>Avada Barbers</div>
          <div>123 New York Street</div>
          <div>New York City</div>
          <div>info@yourwebsite.com</div>
          <div>+1 (555) 555-1212</div>
        </div>
        <p>FOLLOW US</p>
        <div class="social-icons">
          <i class="fa-brands fa-facebook-f"></i>
          <i class="fa-brands fa-twitter"></i>
          <i class="fa-brands fa-youtube"></i>
          <i class="fa-brands fa-instagram"></i>
        </div>
      </div>
      <div>
        <div>
          <img
            class="resize-img"
            src="../assets/img/avadabarbers_footer_appointment_image.png"
            alt="Footer Appointment"
          />
        </div>
        <button>BOOK YOUR APPOINTMENT</button>
      </div>
    </div>

    <div id="bottom-half-footer"></div>
  </div>
</template>

<script>
export default {
  name: "FooterComponent",
};
</script>

<style lang="scss" scoped>
#top-half-footer {
  background-color: #121314;
  text-align: center;
  display: flex;
  justify-content: center;
  column-gap: 118px;
  padding-top: 58px;
  padding-bottom: 75px;

  .resize-img {
    width: 360px;
  }

  .agency-infos {
    color: #686868;
    font-family: Helvetica, Arial;
    font-weight: 100;
    width: 100%;
    margin: 50px 0px 40px 0px;
  }

  .agency-infos div {
    margin-top: 8px;
  }

  p {
    color: #be9359;
    font-family: Helvetica, Arial;
    font-size: 1.05rem;
    font-weight: bold;
    letter-spacing: 1.8px;
    margin: 45px 0px 35px 0px;
  }

  button {
    width: 250px;
    padding: 14px 16px;
    font-size: 0.9rem;
    font-weight: bold;
    background-color: rgba(0, 0, 0, 0);
    color: #be9359;
    border: 2px solid #be9359;
    margin-top: 18px;
  }

  .social-icons {
    color: white;
    display: flex;
    justify-content: center;
    column-gap: 10px;
  }
}

#bottom-half-footer {
  min-height: 120px;
  background-color: #161718;
}
</style>