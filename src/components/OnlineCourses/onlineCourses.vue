<template>
  <div class="accCourses">
      <h1>Popular Online Courses</h1>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Velit voluptate repudiandae quam dolor hic nihil omnis incidunt veniam dolores voluptas! </p>
      <div class="cards">
        <OnlineCoursesCard v-for="(card,index) in onlineCards" :key="index" :card='card'/>
      </div>
      

  </div>
</template>

<script>
import OnlineCoursesCard from './onlineCoursesCard.vue';
export default {
    data() {
        return {
            onlineCards: [
                {
                    img: require("../../assets/img/course-1-f-img.jpg"),
                    title: "Android Developer",
                    price: "free",
                    teacher: "David Sanders",
                    description: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Velit voluptate repudiandae quam dolor hic nihil",
                    subscribed: 1,
                    label: "Programming"
                },
                {
                    img: require("../../assets/img/course-2-f-img.jpg"),
                    title: "Web designing",
                    price: "free",
                    teacher: "Jennifer Powell",
                    description: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Velit voluptate repudiandae quam dolor hic nihil",
                    subscribed: 1,
                    label: "Programming"
                },
                {
                    img: require("../../assets/img/course-3-f-img.jpg"),
                    title: "Financial Modelling",
                    price: "$20",
                    teacher: "Edward Bowman",
                    description: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Velit voluptate repudiandae quam dolor hic nihil",
                    subscribed: 1,
                    label: "Business"
                },
            ]
        };
    },
    components: { OnlineCoursesCard }
}
</script>

<style lang="scss" scoped>
    @import '../../style/main.scss';

    .accCourses {
        text-align: center;
        border-top: .1px solid $primary_border;
        border-bottom: .1px solid $primary_border;
        padding-top: 50px;
        padding-bottom: 50px;
        position: relative;
        

        &::before {

            content:"";
            background-image: url('../../assets/img/page-background-img.png');
            background-repeat: repeat;
            background-size: cover;
            position: absolute;
            opacity: 1;
            z-index: -1;
            top:0px;
            bottom:0;
            left:0;
            right:0;
        }
        
        h1 {
            color: $primary_title;
            margin-bottom: 20px;
        }
        p {
            color: $primary_font;
            padding: 0px 200px;
            margin-bottom: 50px;
        }

        .cards {

            @include myflex('both');
            width: 80%;
            margin: auto;
        }
    }

</style>