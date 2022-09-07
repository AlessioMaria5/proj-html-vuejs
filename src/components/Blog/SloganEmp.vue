<template>
    <div class="slogan">
        <GoTop />
        <div class="img-wrapper">
            <img src="../../assets/img/h5-img-2.jpg">
        </div>
       
        <div class="right-side">
            <h1>Empowering Children to Reach Their Potential.</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam quam excepturi eum laudantium veniam libero adipisci natus, perspiciatis, neque numquam ducimus officiis in iste!</p>
            <div class="eventsCounters">
                <div class="userEventsCounter">
                <div class="eventCounter">168</div>
                <div class="eventTitle">User Stories</div>
            </div>
            <div class="userEventsCounter">
                <div class="eventCounter">347</div>
                <div class="eventTitle">Events</div>
            </div>
            </div>
            
        </div>
      
    </div>
</template>

<script>
import GoTop from '../goTop.vue';
export default {
    components: { GoTop }
}
</script>

<style lang="scss">
    @import '../../style/main.scss';
    
    .slogan {
        @include myflex('both');
        padding: 40px 0px;
        padding-bottom: 40px;
        position: relative;
       

        .img-wrapper {

            align-self: flex-end;
            width: 40%;

            img {
            width: 100%;
            
            object-fit: cover;
            
        }
        }
     

        .right-side {

           width: 35%;

           h1 {
            margin-bottom:20px;
            margin-top: 20px;
            color: $primary_title;
            
           }

           p {
               margin-bottom:20px;
               color: $primary_font;
           }

           .eventsCounters {
               @include myflex('both');
               justify-content: flex-start;
               
               .userEventsCounter {
                   margin-right: 50px;
                   color: $primary_color;

                   .eventCounter {
                       font-size: 2.5em;
                   }
               }
           }
        }
    }

</style>