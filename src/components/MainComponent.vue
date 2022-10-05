<template>
  <div id="main-container">
    <ServicesComponent />
  </div>
</template>

<script>
import ServicesComponent from "@/components/ServicesComponent.vue";

export default {
  name: "MainComponent",

  components: {
    ServicesComponent,
  },
};
</script>

<style lang="scss" scoped>
</style>