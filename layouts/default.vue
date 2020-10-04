<template>
  <div>
    <Header />
    <Nuxt />
    <Footer />
  </div>
</template>
<script>
import Header from "@/components/header.vue";
import Footer from "@/components/footer.vue";

export default {
  components: {
    Header,
    Footer,
  },
};
</script>
<style lang="scss">
@import "~assets/scss/common.scss";
.background {
  position: fixed;
  z-index: 1;
  width: 100%;
  height: 100%;
  overflow: hidden;
  background-color: #000;
  opacity: 0.5;
}
img {
  width: 100%;
}
</style>
