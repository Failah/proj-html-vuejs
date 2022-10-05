<template>
  <div>
    <div id="reviews-section">
      <p>WHAT PEOPLE SAY</p>
      <h2>Reviews</h2>
      <div class="reviews-container">
        <div>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nostrum
            amet quisquam quia, ea, placeat sed temporibus optio nulla repellat
            debitis repellendus nesciunt? Illo, eveniet iure quis et accusantium
            harum ut?
          </p>
          <div>
            <img src="../assets/img/avadabarbers-trimcut-gallery6.jpg" alt="" />
          </div>
          <div class="reviewer-name">John Doe</div>
        </div>
        <div>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nostrum
            amet quisquam quia, ea, placeat sed temporibus optio nulla repellat
            debitis repellendus nesciunt? Illo, eveniet iure quis et accusantium
            harum ut?
          </p>
          <div>
            <img src="../assets/img/avadabarbers-trimcut-gallery6.jpg" alt="" />
          </div>
          <div class="reviewer-name">Pete Jones</div>
        </div>
        <div>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nostrum
            amet quisquam quia, ea, placeat sed temporibus optio nulla repellat
            debitis repellendus nesciunt? Illo, eveniet iure quis et accusantium
            harum ut?
          </p>
          <div>
            <img src="../assets/img/avadabarbers-trimcut-gallery6.jpg" alt="" />
          </div>
          <div class="reviewer-name">Mark Wilson</div>
        </div>
      </div>
    </div>

    <div id="blog-section"></div>
  </div>
</template>

<script>
export default {
  name: "ReviewsAndBlogComponent",
};
</script>

<style lang="scss" scoped>
#reviews-section {
  padding-top: 90px;
  text-align: center;

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
    margin-bottom: 50px;
  }

  .reviews-container {
    width: 1150px;
    margin: 0 auto;
    display: flex;

    p {
      color: #686868;
      font-family: Helvetica, Arial;
      font-weight: 100;
      width: 80%;
      padding-left: 40px;
      margin-bottom: 30px;
    }

    img {
      width: 120px;
      border-radius: 50%;
      margin-bottom: 20px;
    }

    .reviewer-name {
      color: #be9359;
      font-family: Helvetica, Arial;
      font-size: 1.05rem;
      font-weight: bold;
      letter-spacing: 1.8px;
      margin-bottom: 100px;
    }
  }
}
</style>