<template>
  <div class="jumboSlider">
    
        <hgroup>
          <h1>Contemporary Ideas</h1>
          <div class="subtitle">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta tenetur nemo</div>
        </hgroup>
          <a href="#">Register Now</a>
  </div>
</template>

<script>
 
export default {
    components: { }
}
</script>

<style lang="scss">
    @import '../style/main.scss';
    @import '../style/buttons.scss';

    .jumboSlider {
      position:relative;
        @include myflex('both');
        position:relative;
        flex-direction: column;
        text-align:center;
        margin-top: 50px;
        color:white;
        
        
        h1 {

            font-size:4em;
        }

        a {
            @include styleBtn('classic');
            
            
        }
        
    }

</style>