<template>
  <div id="services" class="container mt-5">
    <CCard3 class="alt" title="Search company" />
    <CCard3 title="Registry forms" />
    <CCard3 class="alt" title="Training schedule" />
    <CCard3 title="Search CBP" />
  </div>
</template>

<script>
import cCard3 from "../components/cards/cCard3.vue";
import CCard3 from "../components/cards/cCard3.vue";

export default {
  components: {
    cCard3,
    CCard3,
  },
};
</script>

<style lang="scss">
#services {
}
</style>
