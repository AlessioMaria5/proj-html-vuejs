<template>
  <div class="header">
      <NavBar />
      <JumboSlider />
      
  </div>
</template>

<script>
import NavBar from './navBar.vue';
import JumboSlider from './jumboSlider.vue';
export default {
    name: "iAccHeader",
    components: { NavBar, JumboSlider }
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
            position: absolute;
            opacity: 1;
            z-index: -1;
            top:0;
            bottom:0;
            left:0;
            right:0;
        }
</style>