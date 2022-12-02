<template>
  <TheHeader></TheHeader>
  <TheMain></TheMain>
  <TheMainBanner></TheMainBanner>
  <TheFooter></TheFooter>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import TheMain from "./components/TheMain.vue";
import TheMainBanner from "./components/TheMainBanner.vue";
import TheFooter from "./components/TheFooter.vue";

export default {
  components: { TheHeader, TheMain, TheMainBanner, TheFooter }
}
</script>

<style lang="scss">
@use "./styles/general.scss";
</style>
