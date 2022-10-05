<template>
  <div id="main-container">
    <ServicesComponent />
    <ProductsComponent />
    <ReviewsAndBlogComponent />
  </div>
</template>

<script>
import ServicesComponent from "@/components/ServicesComponent.vue";
import ProductsComponent from "@/components/ProductsComponent.vue";
import ReviewsAndBlogComponent from "@/components/ReviewsAndBlogComponent.vue";

export default {
  name: "MainComponent",

  components: {
    ServicesComponent,
    ProductsComponent,
    ReviewsAndBlogComponent,
  },
};
</script>

<style lang="scss" scoped>
</style>