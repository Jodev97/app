<template>
  <div>
    <!-- HEADER -->
    <header>
      <layout-header />
    </header>

    <!-- BODY -->
    <main class="container mt-3">
      <actions-nav></actions-nav>
      <main-layout>
        <template v-slot:content> <router-view /> </template>
        <template v-slot:sidebarRigth> <c-events /> </template>
      </main-layout>
    </main>

    <!-- FOOTER -->
    <footer>
      <cFooter1 />
    </footer>
  </div>
</template>
<script>
import LayoutHeader from "@/components/headers/LayoutHeader.vue";
import MainLayout from "@/views/MainLayout.vue";
import cFooter1 from "./components/footers/cFooter1.vue";
import CEvents from "./components/cEvents.vue";
import ActionsNav from "./components/navs/ActionsNav.vue";

export default {
  components: { LayoutHeader, MainLayout, cFooter1, CEvents, ActionsNav },
};
</script>
<style lang="scss">
#app {
}
</style>
