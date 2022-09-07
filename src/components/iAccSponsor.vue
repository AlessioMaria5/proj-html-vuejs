<template>
  <div class="sponsor">
      <div v-for="(sponsor, index) in sponsors" :key="index" class="sponsor-wrapper">
          <img :src="sponsor.img" alt="">
      </div>
  </div>
</template>

<script>
export default {
    name: 'iAccSponsor',
    data() {
        return {

            sponsors: [
                {
                    img: require('../assets/img/h5-client-1.png'),
                    name: 'sponsor name'
                },
                {
                    img: require('../assets/img/h5-client-2.png'),
                    name: 'sponsor name'
                },
                {
                    img: require('../assets/img/h5-client-3.png'),
                    name: 'sponsor name'
                },
                {
                    img: require('../assets/img/h5-client-4.png'),
                    name: 'sponsor name'
                },
            ]
        }
    }
}
</script>

<style lang="scss">
    @import '../style/main.scss';
    .sponsor {
        display: flex;
        justify-content: space-around;
        padding: 40px;
        border-top:  .1px solid $primary_border;
        border-bottom:  .1px solid $primary_border;
        
        

        .sponsor-wrapper {
            width: calc(100% / 4);
            

            img {

                width: 100%

            }
        }
    }
</style>