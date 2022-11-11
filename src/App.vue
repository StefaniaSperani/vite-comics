<script>
import HeaderComp from './components/HeaderComp.vue';
import BodyComp from './components/BodyComp.vue';
import FooterComp from './components/FooterComp.vue';
import Footer2Comp from './components/Footer2Comp.vue';
import MerchComp from './components/MerchComp.vue';
import JumboComp from './components/JumboComp.vue';
export default {
  components: {
    HeaderComp,
    BodyComp,
    FooterComp,
    Footer2Comp,
    MerchComp,
    JumboComp
  }
}
</script>

<template>
  <HeaderComp />
  <main>
    <JumboComp />
    <BodyComp />
    <MerchComp />
  </main>
  <FooterComp />
  <Footer2Comp />
</template>

<style lang="scss" scoped>

</style>
