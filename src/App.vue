<template>
  <TheHeader></TheHeader>
  <TheMain></TheMain>
  <TheMainBanner></TheMainBanner>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import TheMain from "./components/TheMain.vue";
import TheMainBanner from "./components/TheMainBanner.vue";

export default {
  components: { TheHeader, TheMain, TheMainBanner, }
}
</script>

<style lang="scss">
@use "./styles/general.scss";
</style>
