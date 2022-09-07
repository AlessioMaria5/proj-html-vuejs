<template>
  <div class="cards-section">
      <SingleCard v-for="(card, index) in cardsData" :key="index"  :cardTitle='card.title' :cardUrl='card.icon'/>
  </div>
</template>

<script>
import SingleCard from './SingleCard.vue';
export default {
    components: { SingleCard },
    data() {
      return {

        cardsData: [
          {
            icon: require('/src/assets/img/h5-custom-icon-1.png'),
            title: 'Languages'
          },

          {
            icon: require('/src/assets/img/h5-custom-icon-2.png'),
            title: 'Software'
          },

          {
            icon: require('/src/assets/img/h5-custom-icon-3.png'),
            title: 'Business'
          },

          {
            icon: require('/src/assets/img/h5-custom-icon-4.png'),
            title: 'Chemistry'
          },

          {
            icon: require('/src/assets/img/h5-custom-icon-5.png'),
            title: 'Science'
          },

          {
            icon: require('/src/assets/img/h5-custom-icon-6.png'),
            title: 'DIY&Craft'
          },

        ]
      }
    }
}
</script>

<style lang="scss">
@import '../../style/main.scss';

  .cards-section {

    @include myflex('both')
    
  }

</style>