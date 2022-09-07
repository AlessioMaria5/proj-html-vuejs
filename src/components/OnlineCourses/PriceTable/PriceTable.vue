<template>
  <div class="priceTable">
    <h1>Pricing Plans</h1>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Velit</p>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
    @import '../../../style/main.scss';

    .priceTable {
        text-align: center;

        &::before {
            
            @include backgrounds('primary');
            background-image: url('../../../assets/img/page-background-img.png');

        }

        h1 {

            color: $primary_title;
            margin-bottom:20px;
        }

        p {
            color: $primary_font;
        }
    }

</style>