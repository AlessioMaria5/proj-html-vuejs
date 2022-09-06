<template>
  <div id="main">
      <IAccCards />
      <div class="events">Events</div>
      <div class="testimonials">Testimonials</div>
      <div class="learning">Learning</div>
      <div class="courses">Courses</div>
      <div class="pricing-plans">Pricing Plans</div>
      <div class="sponsor">Sponsor</div>

  </div>
</template>

<script>
import IAccCards from './CardSection/iAccCards.vue';
export default {
    name: "iAccMain",
    components: { IAccCards }
}
</script>

<style>

</style>