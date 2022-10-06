<template>
  <header>
    <!-- this are the 2 icons at the top right of the screen in the header -->
    <div id="right-outside-icons">
      <div>
        <img src="../assets/img/header-demos.png" alt="Demo" />
      </div>
      <div>
        <img src="../assets/img/header-onsale.png" alt="" />
      </div>
    </div>

    <!-- the top navbar with hamburger menu (openable) -->
    <div id="header-container">
      <div class="top-navbar">
        <div>
          <img src="../assets/img/avadabarbers-logo-x1.png" alt="Avada Logo" />
        </div>
        <div>
          <a href="#top-half-footer"
            ><i class="fa-solid fa-cart-shopping"></i
          ></a>
          <div class="header-navbar">
            <i @click="toggleSearchInput" class="fa-solid fa-bars"></i>
            <div
              id="toggle-menu"
              :class="{ toggle: toggleIndex === true }"
              class="input"
            >
              <!-- nav links in the page -->
              <nav v-if="toggleIndex === true">
                <a href="#services-container">Services</a>
                <a href="#top-half-products">Products</a>
                <a href="#reviews-section">Reviews</a>
              </nav>
            </div>
          </div>
        </div>
      </div>

      <!-- this is the entire header section -->
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

  data() {
    return {
      toggleIndex: false,
    };
  },

  methods: {
    toggleSearchInput() {
      console.log("search input clicked");
      this.toggleIndex = !this.toggleIndex;
    },
  },
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

      &:hover {
        filter: brightness(150%);
        cursor: pointer;
      }
    }
  }

  #header-container {
    max-width: 1150px;
    margin: 0 auto;

    .top-navbar > div:nth-child(2) {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

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
          padding-right: 10px;
        }

        &:hover {
          transition: color 0.3s linear;
          color: #686868;
        }
      }

      .header-navbar {
        right: 15px;
        position: relative;
        display: inline-block;

        nav {
          height: 100%;
          display: flex;
          justify-content: center;
          align-items: center;
          column-gap: 20px;

          a {
            text-decoration: none;
            color: white;
            font-family: "Abril", Helvetica, Arial;
            font-size: 1.1rem;

            &:hover {
              transform: scale(1.1);
            }
          }
        }

        #toggle-menu {
          width: 0px;
          height: 34px;
          box-shadow: none;
          border: 1px solid transparent;
          outline: none;
          padding-left: 35px;
          font-size: 16px;
          transition: 0.3s ease all;

          &.toggle {
            width: 280px;
          }
        }

        i {
          width: 18px;
          left: 8px;
          top: 50%;
          transform: translateY(-50%);
          position: absolute;
          cursor: pointer;
          font-size: 1.9rem;
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
      font-family: "Abril", Helvetica, Arial;
      font-weight: 100;
      font-size: 5rem;
      letter-spacing: 4px;
      color: white;
    }

    #separation-bar {
      height: 4px;
      width: 48%;
      background-color: #be9359;
      margin: 25px 0px 28px 0px;
    }

    .under-comment {
      color: #686868;
      font-family: "Palanquin", Helvetica, Arial;
      font-size: 1.5rem;
      letter-spacing: 0.5px;
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

      &:hover {
        cursor: pointer;
        transform: scale(1.02);
        filter: brightness(130%);
      }
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