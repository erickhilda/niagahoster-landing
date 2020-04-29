<template>
  <div class="home">
    <app-banner />
    <!-- <app-feature /> -->
    <app-package />
    <app-tech-stack />
    <app-laravel-support />
    <app-footer />
  </div>
</template>

<script>
import AppBanner from "@/components/AppBanner";
// import AppFeature from "@/components/AppFeature";
import AppPackage from "@/components/AppPackage";
import AppTechStack from "@/components/AppTechStack";
import AppLaravelSupport from "@/components/AppLaravelSupport";
import AppFooter from "@/components/AppFooter";

export default {
  name: "Home",
  components: {
    AppBanner,
    // AppFeature,
    AppPackage,
    AppTechStack,
    AppLaravelSupport,
    AppFooter
  }
};
</script>

<style lang="scss">
.section__title {
  font-family: "Montserrat", sans-serif;
  font-weight: 700;
  color: #4c4c4c;
  font-size: 24px;
}

.section__subtitle {
  font-family: "Montserrat", sans-serif;
  font-weight: 500;
  color: #4c4c4c;
  font-size: 22px;
}

.section__wrapper {
  padding: 30px 0px;
}
</style>
