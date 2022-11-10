<script>
import HeaderComp from './components/HeaderComp.vue';
import BodyComp from './components/BodyComp.vue';
import FooterComp from './components/FooterComp.vue';
import Footer2Comp from './components/Footer2Comp.vue';
export default {
  components: {
    HeaderComp,
    BodyComp,
    FooterComp,
    Footer2Comp
  }
}
</script>

<template>
  <HeaderComp />
  <main>
    <BodyComp />
  </main>
  <FooterComp />
  <Footer2Comp />
</template>

<style lang="scss" scoped>

</style>
