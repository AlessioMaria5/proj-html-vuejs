<template>
  <div class="header">
      <NavBar />
      <JumboSlider />
      <SliderSpot />
  </div>
</template>

<script>
import NavBar from './navBar.vue';
import JumboSlider from './jumboSlider.vue';
import SliderSpot from './sliderSpot.vue';
export default {
    name: "iAccHeader",
    components: { NavBar, JumboSlider, SliderSpot }
}
</script>

<style lang="scss">


    .header {        
        height: 550px;
        position:relative;
        background-color: rgba(0,0,0,0.2);
        padding-top: 20px;
    }

    .header::before {
            content:"";
            background-image: url('../assets/img/course-9-f-img.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            position: absolute;
            opacity: 1;
            z-index: -1;
            top:0;
            bottom:0;
            left:0;
            right:0;
        }
</style>