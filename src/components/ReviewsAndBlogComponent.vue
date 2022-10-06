<template>
  <div>
    <div id="reviews-section">
      <!-- this is the top half with all the reviews displayed non-dinamically via js but typed manually in the html -->
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
            <img src="../assets/img/avadabarbers-trimcut-gallery7.jpg" alt="" />
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
            <img src="../assets/img/avadabarbers-trimcut-gallery3.jpg" alt="" />
          </div>
          <div class="reviewer-name">Mark Wilson</div>
        </div>
      </div>
    </div>

    <div id="blog-section">
      <!-- this is the triangle shaped div that separes some sections -->
      <div class="triangle-down"></div>

      <!-- this is the bottom half part of the section with the blogs -->
      <p>TALES FROM THE BARBER SHOP</p>
      <h2>Recent Blog Posts</h2>
      <div id="blog-post-container">
        <div>
          <div>
            <img
              src="../assets/img/avadabarbers-second-blog-700x441.jpg"
              alt=""
            />
          </div>
          <h3>Avada Barbers Now Open</h3>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nostrum
            amet quisquam quia!
          </p>
        </div>
        <div>
          <div>
            <img
              src="../assets/img/avadabarbers-choosing-blog-700x441.jpg"
              alt=""
            />
          </div>
          <h3>Choosing The Right Barber</h3>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nostrum
            amet quisquam quia!
          </p>
        </div>
        <div>
          <div>
            <img
              src="../assets/img/avadabarbers-ourservice-blog-700x441.jpg"
              alt=""
            />
          </div>
          <h3>Quick Service Guide</h3>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nostrum
            amet quisquam quia!
          </p>
        </div>
      </div>
      <button>READ MORE FROM OUR BLOG</button>
    </div>
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

#blog-section {
  background-color: #f5f5f5;
  position: relative;
  padding-top: 200px;
  text-align: center;

  // this is the triangle shaped div that separes some sections
  .triangle-down {
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 0;
    border-left: 950px solid transparent;
    border-right: 950px solid transparent;
    border-top: 100px solid white;
  }

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

  #blog-post-container {
    max-width: 1150px;
    margin: 0 auto;
    display: flex;
    column-gap: 30px;

    img {
      width: 100%;
    }

    h3 {
      color: #be9359;
      font-family: "Abril", Helvetica, Arial;
      font-size: 2rem;
      font-weight: 100;
      margin-top: 20px;
      margin-bottom: 15px;
    }

    p {
      color: #686868;
      font-family: Helvetica, Arial;
      font-weight: 100;
    }
  }

  button {
    margin-top: 70px;
    margin-bottom: 120px;
    width: 350px;
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