<template>
  <div id="main">
      <IAccCards />
      <IAccBlog />
      <SloganEmp />
      <IAccTestimonials />
      <IAccLearning />
      <OnlineCourses />
      <PriceTable />
      <div class="pricing-plans">Pricing Plans</div>
      <div class="sponsor">Sponsor</div>

  </div>
</template>

<script>
import IAccCards from './CardSection/iAccCards.vue';
import IAccBlog from './Blog/iAccBlog.vue';
import SloganEmp from './Blog/SloganEmp.vue';
import IAccTestimonials from './Testimonials/iAccTestimonials.vue';
import IAccLearning from './iAccLearning.vue';
import OnlineCourses from './OnlineCourses/onlineCourses.vue';
import PriceTable from './OnlineCourses/PriceTable/PriceTable.vue';
export default {
    name: "iAccMain",
    components: { IAccCards, IAccBlog, SloganEmp, IAccTestimonials, IAccLearning, OnlineCourses, PriceTable }
}
</script>

<style>

</style>