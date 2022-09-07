<template>
  <div class="card">
    <div class="card-img">
      <img :src="card.img" alt="">
    </div>
    <hgroup>
      <h3>{{card.title}}</h3>
      <h5>{{card.teacher}}</h5>
      <span class="label">{{card.price}}</span>
    </hgroup>
    <p>{{card.description}}</p>
    <div class="card-footer">
      <span>{{'x' + card.subscribed}}</span>
      <span>{{'x' + card.label}}</span>
    </div>
  </div>
</template>

<script>
export default {
    props: {
      
      card: Object,
    }
}
</script>

<style lang="scss" scoped>
  @import '../../style/main.scss';

  .card {
    border: 0.1px solid $primary_border;  
    width: calc(100% / 3);
    background-color: white;
    

    hgroup {
      position: relative;

      h1,h2,h3,h4,h5 {
      text-align: start;
      font-size: 0.8em;
      }
      h3 {
        color: $primary_title;
      }
      h5 {
        color: $secondary_font;
      }

      span {
      @include priceLabel('secondary');
      text-transform: uppercase;
      right:10px;
      top:10px;      
    }
    }

    p {
      text-align: start;
      color: $primary_font;
      font-size: 0.8em;
      line-height: 18px;
      margin-top:10px;
    }

    hgroup, p {

      padding: 10px;
    }


    .card-img {

      width: 100%;

      img {
        object-fit: cover;
        width: 100%;
      }
    }
    .card-footer {

      font-size: .7em;
      text-transform: uppercase;
      text-align: start;
      margin-left: 10px;
      margin-top: 10px;
      padding-bottom: 20px;
      color: $secondary_font;

      span {

        margin-right: 10px;
      }
    }

  }

</style>