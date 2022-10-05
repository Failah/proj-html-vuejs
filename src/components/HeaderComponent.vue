<template>
  <header>
    <div id="header-container">
      <div class="top-navbar">
        <div>
          <img src="../assets/img/avadabarbers-logo-x2.png" alt="Avada Logo" />
        </div>
        <div></div>
      </div>
      <div class="center-header">
        <div></div>
        <div></div>
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

  #header-container {
    max-width: 1150px;
    margin: 0 auto;

    .top-navbar {
      width: 100%;
      padding-top: 30px;
      display: flex;
      justify-content: space-between;

      img {
        width: 180px;
      }
    }
  }
}
</style>