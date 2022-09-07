<template>
  <div id="main">
      <IAccCards />
      <IAccBlog />
      <SloganEmp />
      <IAccTestimonials />
      <IAccLearning />
      <!-- <div class="courses">Courses</div>
      <div class="pricing-plans">Pricing Plans</div>
      <div class="sponsor">Sponsor</div> -->

  </div>
</template>

<script>
import IAccCards from './CardSection/iAccCards.vue';
import IAccBlog from './Blog/iAccBlog.vue';
import SloganEmp from './Blog/SloganEmp.vue';
import IAccTestimonials from './Testimonials/iAccTestimonials.vue';
import IAccLearning from './iAccLearning.vue';
export default {
    name: "iAccMain",
    components: { IAccCards, IAccBlog, SloganEmp, IAccTestimonials, IAccLearning }
}
</script>

<style>

</style>