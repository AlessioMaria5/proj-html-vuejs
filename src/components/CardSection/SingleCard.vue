<template>
  <div class="SingleCard">
        <img :src="cardUrl">
        <label for="i">{{cardTitle}}</label>
  </div>
</template>

<script>
export default {

    name: 'singleCard',
    props: {
        
        cardTitle: String,
        cardUrl: String
        
    }

}
</script>

<style lang="scss" scoped>
    @import '../../style/main.scss';

    .SingleCard {
        display:flex;
        flex-direction:column;
        align-items: center;

        padding: 50px 0px;
        background-color: $secondary_bg;
        width: calc(80% / 6);

        margin-top:50px;

        img {
            width: 40%;
            margin-bottom:20px;
        }
    }

</style>