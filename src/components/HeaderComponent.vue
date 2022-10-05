<template>
  <header>
    <div id="right-outside-icons">
      <div>
        <img src="../assets/img/header-demos.png" alt="Demo" />
      </div>
      <div>
        <img src="../assets/img/header-onsale.png" alt="" />
      </div>
    </div>
    <div id="header-container">
      <div class="top-navbar">
        <div>
          <img src="../assets/img/avadabarbers-logo-x1.png" alt="Avada Logo" />
        </div>
        <div>
          <i class="fa-solid fa-cart-shopping"></i>
          <i class="fa-solid fa-bars"></i>
        </div>
      </div>

      <div class="center-header">
        <div>
          <h1>Barber Shop</h1>
          <div id="separation-bar"></div>
          <div class="under-comment">The Pinnacle of Male Grooming</div>
          <button>LEARN MORE</button>
        </div>
        <div>
          <img
            src="../assets/img/avadabarbers_hero_focalmirror-600x825.png"
            alt="Avada Barbers"
          />
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
};
</script>

<style lang="scss" scoped>
header {
  min-height: 965px;
  background-image: url("../assets/img/avadabarbers-homepage-hero-bg.jpg");
  background-size: cover;

  #right-outside-icons {
    position: absolute;
    right: 0.8%;
    top: 16%;
    display: flex;
    flex-direction: column;
    row-gap: 7px;

    div {
      height: 65px;
      width: 65px;
      border-radius: 7px;
      background-color: white;
      display: flex;
      justify-content: center;
      align-items: center;
    }
  }

  #header-container {
    max-width: 1150px;
    margin: 0 auto;

    .top-navbar {
      width: 100%;
      padding-top: 30px;
      display: flex;
      justify-content: space-between;
      align-items: center;

      i {
        color: white;

        &.fa-cart-shopping {
          font-size: 1.1rem;
          margin-right: 25px;
        }

        &.fa-bars {
          font-size: 1.6rem;
          padding-right: 10px;
        }
      }
    }
  }

  .center-header {
    height: 750px;
    display: flex;
    column-gap: 70px;
  }

  .center-header div:nth-child(1) {
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;

    h1 {
      font-size: 6rem;
      color: white;
    }

    #separation-bar {
      height: 4px;
      width: 48%;
      background-color: #be9359;
      margin: 25px 0px 28px 0px;
    }

    .under-comment {
      color: grey;
      font-size: 1.5rem;
      font-weight: lighter;
      margin-top: 5px;
      margin-bottom: 42px;
    }

    button {
      width: 200px;
      padding: 18px 20px;
      font-size: 1.1rem;
      background-color: rgba(0, 0, 0, 0);
      color: #be9359;
      border: 2px solid #be9359;
    }
  }

  .center-header div:nth-child(2) {
    img {
      width: 100%;
      height: 100%;
    }
  }
}
</style>