<template>
  <TheHeader></TheHeader>
  <TheMain></TheMain>
  <TheMainBanner></TheMainBanner>
  <TheFooter></TheFooter>
  <TheFooterSmall></TheFooterSmall>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import TheMain from "./components/TheMain.vue";
import TheMainBanner from "./components/TheMainBanner.vue";
import TheFooter from "./components/TheFooter.vue";
import TheFooterSmall from "./components/TheFooterSmall.vue";

export default {
  components: { TheHeader, TheMain, TheMainBanner, TheFooter, TheFooterSmall }
}
</script>

<style lang="scss">
@use "./styles/general.scss";
</style>
