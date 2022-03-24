<template>
  <div id="app">
    <HeaderMolisana />
    <MainGrid />
    <FooterMolisana />
  </div>
</template>

<script>
import HeaderMolisana from '@/components/HeaderMolisana.vue'
import MainGrid from '@/components/MainGrid.vue'
import FooterMolisana from '@/components/FooterMolisana.vue'

export default {
  name: 'App',
  components: {
    HeaderMolisana,
    MainGrid,
    FooterMolisana
  }
}
</script>

<style lang="scss">
@import "@/assets/styles/style.scss";
</style>
