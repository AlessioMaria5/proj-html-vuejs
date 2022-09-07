<template>
  <div class="blog">
      <h1>The Trusted Name <br> for In-Home Tutoring.</h1>
      <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur ipsam necessitatibus dolores iusto natus architecto ipsum autem ducimus error. Nulla vel odio, neque provident sint commodi vitae vero quas voluptatibus!</p>
      <a href="#">Learn More</a>
      <div class="blogImg">
        <img src="../../assets/img/h5-img-1.jpg" alt="students with books">
      </div>
      
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">

    @import '../../style/main.scss';

    .blog {
        padding: 50px 50px 0px 50px;
        
        
        h1 {
            margin-bottom: 15px;
            color: $primary_title;
        }

        p {
            margin-bottom: 15px;
            color: $primary_font;
        }

        a {
            text-decoration: none;
            color: $primary_color;
            text-transform: uppercase;
        }

        .blogImg {
            img {
                width: 100%;
            }
        }
    }

</style>