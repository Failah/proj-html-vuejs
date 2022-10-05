<template>
  <div id="app">
    <HeaderComponent />
    <MainComponent />
  </div>
</template>

<script>
import HeaderComponent from "@/components/HeaderComponent.vue";
import MainComponent from "@/components/MainComponent.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
    MainComponent,
  },
};
</script>

<style lang="scss">
@import "./css/generics.scss";

@font-face {
  font-family: "Elephant";
  src: local("elephant"), url(./fonts/elephant.ttf) format("truetype");
}

@font-face {
  font-family: "Abril";
  src: local("abril"), url(./fonts/abril.ttf) format("truetype");
}

@font-face {
  font-family: "Palanquin";
  src: local("palanquin"), url(./fonts/Palanquin-Thin.ttf) format("truetype");
}
</style>
