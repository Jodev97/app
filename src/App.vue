<template>
  <div>
    <!-- HEADER -->
    <header>
      <layout-header />
    </header>

    <!-- BODY -->
    <main class="container">
      <main-layout>
        <template v-slot:content> <router-view /> </template>
        <template v-slot:sidebarRigth> sidebar </template>
      </main-layout>
    </main>

    <!-- FOOTER -->
    <footer></footer>
  </div>
</template>
<script>
import LayoutHeader from "@/components/headers/LayoutHeader.vue";
import MainLayout from "@/views/MainLayout.vue";
export default {
  components: { LayoutHeader, MainLayout },
};
</script>
<style lang="scss">
#app {
}
</style>
