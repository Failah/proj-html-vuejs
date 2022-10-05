<template>
  <div id="app">
    <HeaderComponent />
  </div>
</template>

<script>
import HeaderComponent from "@/components/HeaderComponent.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
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
</style>
