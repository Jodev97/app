<template>
  <div id="HomeView" class="row">
    <section class="my-5" style="min-height: 250px">
      <h2 class="row my-5">CHAMBER NEWS</h2>
      <CCard2 />
    </section>
    <section class="container">
      <h2 class="row my-5">CHAMBER NEWS</h2>
      <div class="row">
        <cCard1 image="bg_1.png" class="col-6" />
        <cCard1 image="bg_2.jpg" class="col-6" />
      </div>
    </section>
    <section class="my-5">
      <h2 class="row my-5">CHAMBER NEWS</h2>
      <div class="row">
        <cCard1 image="bg_1.png" class="col-4" />
        <cCard1 image="bg_2.jpg" class="col-4" />
        <cCard1 image="bg_2.jpg" class="col-4" />
      </div>
    </section>
  </div>
</template>

<script>
import cCard1 from "../components/cards/cCard1.vue";
import cCard2 from "../components/cards/cCard2.vue";
import CCard2 from "../components/cards/cCard2.vue";

export default {
  name: "HomeView",
  components: { cCard1, cCard2, CCard2 },
};
</script>
<style lang="scss">
#HomeView {
  h2 {
    border-bottom: 2px solid #07367793;
  }
  section {
    min-height: 400px;
  }
}
</style>
