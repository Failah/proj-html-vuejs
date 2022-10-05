<template>
  <div>
    <div id="top-half-footer"></div>

    <div id="bottom-half-footer"></div>
  </div>
</template>

<script>
export default {
  name: "FooterComponent",
};
</script>

<style lang="scss" scoped>
#top-half-footer {
  min-height: 485px;
  background-color: #121314;
}

#bottom-half-footer {
  min-height: 120px;
  background-color: #161718;
}
</style>