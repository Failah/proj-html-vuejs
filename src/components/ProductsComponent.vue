<template>
  <div>
    <!-- this in the top half of the products section -->
    <div id="top-half-products">
      <p>WE HAVE YOU COVERED</p>
      <h2>Avada Grooming Products</h2>
      <!-- here are all the products generated dinamically using array in data.js -->
      <div>
        <div v-for="product in products" :key="product.name">
          <div>
            <img
              :src="require(`../assets/img/${product.image}`)"
              :alt="product.name"
            />
          </div>
          <h3>
            {{ product.name }}
          </h3>
          <span>
            {{ product.price }}
          </span>
        </div>
      </div>
      <div>
        <button>SHOP OUR PRODUCT RANGE</button>
      </div>
    </div>

    <!-- this is the bottom half of the same products section -->
    <div id="bottom-half-products">
      <!-- this is the "out of top border" box with the featured monthly product -->
      <div class="featured-product">
        <div>
          <img src="../assets/img/shaving_butter.png" alt="" />
        </div>
        <div>
          <p>THIS MONTHS FEATURED PRODUCT</p>
          <h2>Shaving Butter</h2>
          <span
            >Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quo
            consectetur laborum tempora magni maiores aspernatur dignissimos
            aperiam consequuntur, hic obcaecati deleniti!</span
          >
          <div>
            <button>BUY NOW</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { products } from "@/data.js";

export default {
  name: "ProductsComponent",

  data() {
    return {
      products: products,
    };
  },
};
</script>

<style lang="scss" scoped>
// skinning of the top half of the products component
#top-half-products {
  min-height: 1035px;
  text-align: center;
  background-image: url("../assets/img/avadabarbers-reviewsbackground.jpg");
  background-size: cover;
  background-position-x: -250px;
  padding-top: 100px;

  p {
    color: #be9359;
    font-family: Helvetica, Arial;
    font-size: 1.05rem;
    font-weight: bold;
    letter-spacing: 1.8px;
  }

  h2 {
    font-family: "Abril", Helvetica, Arial;
    font-weight: 100;
    font-size: 4.4rem;
    letter-spacing: 2px;
    color: #b1b1b1;
    margin-top: 5px;
    margin-bottom: 80px;
  }

  > div {
    display: flex;
    justify-content: center;

    img {
      width: 420px;
    }

    h3 {
      height: 45px;
      color: #be9359;
      font-family: "Abril", Helvetica, Arial;
      font-size: 2rem;
      font-weight: 100;
      margin-bottom: 15px;
    }

    span {
      color: #be9359;
      font-family: Helvetica, Arial;
      font-size: 1.2rem;
      line-height: 2rem;
    }
  }

  button {
    margin-top: 100px;
    width: 300px;
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

// skinning of the bottom half of the products component
#bottom-half-products {
  min-height: 495px;
  background-color: white;
  position: relative;

  .featured-product {
    width: 1150px;
    border-top: 4px solid #be9359;
    position: absolute;
    transform: translate(-50%, 0);
    left: 50%;
    top: -50px;
    display: flex;

    p {
      color: #be9359;
      font-family: Helvetica, Arial;
      font-size: 1.05rem;
      font-weight: bold;
      letter-spacing: 1.8px;
    }

    h2 {
      font-family: "Abril", Helvetica, Arial;
      font-weight: 100;
      font-size: 4.4rem;
      letter-spacing: 2px;
      color: #b1b1b1;
      margin-top: 5px;
      margin-bottom: 35px;
    }

    span {
      display: inline-block;
      width: 80%;
      color: #686868;
      font-family: Helvetica, Arial;
      font-weight: 100;
      line-height: 1.7rem;
    }
  }
}

// just regulate div's width inside the featured product and skin the separately
.featured-product > div:first-child {
  width: 40%;
  background-image: url("../assets/img/avadabarbers-cta-background.jpg");
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;

  img {
    width: 90%;
  }
}

.featured-product > div:nth-child(2) {
  width: 60%;
  background-color: #121413;
  padding: 70px 0px 0px 50px;

  button {
    margin-top: 25px;
    margin-bottom: 70px;
    width: 180px;
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
</style>