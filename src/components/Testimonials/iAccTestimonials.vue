<template>
  <div class="testimonials">
      <div class="img-wrapper">
          <img src="../../assets/img/testimonials-standard-1.png" alt="">
      </div>
      <blockquote>"Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem, explicabo maxime. Ad sequi quae illo vitae hic at architecto expedita porro, magni dolores beatae placeat. Sint, inventore. Excepturi, alias mollitia?"</blockquote>
      <hgroup>
          <h3 class="testimonialName">Joan Collins</h3>
          <h4 class="testimonialRole">Student</h4>
      </hgroup>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
    @import '../../style/main.scss';

    .testimonials {
        @include myflex('both');
        position:relative;
        flex-direction:column;
        padding: 50px 150px;
        color: white;

        &::before{
            content:"";
            background-image: url('../../assets/img/h5-parallax-img-1.png');
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

        hgroup, blockquote {
            text-align: center;
            margin-bottom: 0px;

            h3, h4 {
                margin-bottom: 10px;
            }
        }
    }

</style>