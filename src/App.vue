<template>
  <div>
    <!-- HEADER -->
    <header>
      <layout-header />
    </header>

    <!-- BODY -->
    <main class="container mt-3 mb-5">
      <main-layout>
        <template v-slot:content>
          <Transition name="slide-fade">
            <router-view />
          </Transition>
        </template>
        <template v-slot:sidebarRigth> <c-events /> </template>
      </main-layout>
    </main>

    <!-- FOOTER -->
    <footer class="mt-5">
      <cFooter1 />
    </footer>
  </div>
</template>
<script>
import LayoutHeader from "@/components/headers/LayoutHeader.vue";
import MainLayout from "@/views/MainLayout.vue";
import cFooter1 from "./components/footers/cFooter1.vue";
import CEvents from "./components/cEvents.vue";

export default {
  components: { LayoutHeader, MainLayout, cFooter1, CEvents },
};
</script>
<style lang="scss">
#app {
  .slide-fade-enter-active {
    transition: all 0.3s ease-out;
  }

  .slide-fade-leave-active {
    transition: all 0.3s cubic-bezier(1, 0.5, 0.8, 1);
  }

  .slide-fade-enter-from,
  .slide-fade-leave-to {
    transform: translateX(20px);
    opacity: 0;
  }
}
</style>
