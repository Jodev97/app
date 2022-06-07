<template>
  <div id="HomeView" class="container">
    <section class="my-5" style="min-height: 250px">
      <h2 class="row my-5">FEATURED NEWS</h2>
      <CCard2 />
    </section>
    <section class="container">
      <h2 class="row my-5">CHAMBER NEWS</h2>
      <div class="row">
        <cCard1
          image="bg_1.png"
          class="col-lg-6 col-sm-12"
          title="CHAMBER WEBINAR SERIES JULY 2021"
          content="Willemstad­– Curaçao Chamber of Commerce & Industry continues to
                support (potential) entrepreneurs by offering free webinar
                series. The first webinar “Bureau Intellectual Property” was
                presented by Mr."
          tag="READ MORE"
          date="13th and 15th of July"
        />
        <cCard1
          image="bg_2.jpg"
          class="col-lg-6 col-sm-12"
          title="CHAMBER WEBINARS SERIES APRIL 2021"
          content="Willemstad– Curaçao Chamber of Commerce & Industry continues to support potential entrepreneurs during the pandemic and lockdown by offering free webinar series."
          tag="READ MORE"
          date="On the 1st of April"
        />
      </div>
    </section>
    <section class="my-5">
      <h2 class="row my-5">
        <i class="las la-angle-right" style="color: red; width: 6%"></i
        >HIGHLIGHTS
      </h2>
      <div class="row">
        <cCard1
          image="magazine_4.png"
          class="col-4"
          title="BUSINESS INFO GUIDE"
          content="Curaçao Information Guide (B.I.G.) is the most complete source of 
          information for companies and individuals seeking to do business in and through Curaçao..."
          tag="READ MORE"
        />
        <cCard1
          image="curacao.png"
          class="col-4"
          title="ALL ABOUT CURAÇAO"
          content="Curaçao is located approximately 35 miles off the northwestern coast of Venezuela. 
          The island is about 444 sq."
          tag="READ MORE"
        />
        <cCard1
          image="ec.png"
          class="col-4"
          title="TRAINING & ADVICE"
          content="Especially for the Small Business we have Empresa Chiki. We provide training and advice 
          for everyone. Check out the information and training schedule."
          tag="READ MORE"
        />
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
#cCard1 {
  font-size: 13px;
}
</style>
