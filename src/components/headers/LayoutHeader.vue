<template>
  <section id="main-header" class="container-flux position-relative">
    <main-nav></main-nav>
    <!-- content -->
    <MainHeader v-if="$route.name == 'home'" />
    <AboutHeader v-if="$route.name == 'about'" />
  </section>
</template>

<script>
import MainNav from "@/components/navs/MainNav.vue";
import MainHeader from "@/components/headers/MainHeader.vue";
import AboutHeader from "@/components/headers/AboutHeader.vue";
export default {
  components: {
    MainNav,
    MainHeader,
    AboutHeader,
  },
};
</script>

<style lang="scss">
#main-header {
  min-height: 500px;
  background-image: url("@/assets/bg_1.png");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
