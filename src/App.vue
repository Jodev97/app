<template>
  <div>
    <!-- HEADER -->
    <header>
      <layout-header />
    </header>

    <!-- BODY -->
    <main class="container mt-3">
      <main-layout>
        <template v-slot:content> <router-view /> </template>
        <template v-slot:sidebarRigth> <cList1 /> </template>
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
import cList1 from "./components/lists/cList1.vue";
import cFooter1 from "./components/footers/cFooter1.vue";

export default {
  components: { LayoutHeader, MainLayout, cList1, cFooter1 },
};
</script>
<style lang="scss">
#app {
}
</style>
