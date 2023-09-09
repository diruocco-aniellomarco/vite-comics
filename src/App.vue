<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFouter from "./components/AppFouter.vue";

export default {
  components: { AppHeader, AppMain, AppFouter },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFouter />
</template>

<style lang="scss">
@use "./style/general.scss" as *;
</style>
