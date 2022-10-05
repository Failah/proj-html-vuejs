<template>
  <div id="main-container">
    <ServicesComponent />
    <ProductsComponent />
  </div>
</template>

<script>
import ServicesComponent from "@/components/ServicesComponent.vue";
import ProductsComponent from "@/components/ProductsComponent.vue";

export default {
  name: "MainComponent",

  components: {
    ServicesComponent,
    ProductsComponent,
  },
};
</script>

<style lang="scss" scoped>
</style>