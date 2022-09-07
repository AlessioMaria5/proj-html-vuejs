<template>
  <div class="sliderSpot">
      <div class="circle"></div>
      <div class="circle active"></div>
      <div class="circle"></div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
    .sliderSpot {
        position:absolute;
        bottom: 30px;
        left: calc(50% - 42.5px);
        display: flex;
        gap: 20px;

        .circle {

            border-radius: 50%;
            width: 15px;
            height: 15px;
            background-color: rgb(211, 211, 211);
            
         }  
         .active {
            
            background-color:white;
        }

        }
    
</style>