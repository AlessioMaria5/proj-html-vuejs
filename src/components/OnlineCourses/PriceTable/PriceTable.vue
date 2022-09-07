<template>
  <div class="priceTable">
    <h1>Pricing Plans</h1>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Velit</p>

      <div class="planTable">
        <ul>
            <li>Save up to 40% by paying weekly</li> 
            <li>Number of courses</li>
            <li>Time</li>
            <li>Web Designing</li>
            <li>Human-Centered Design</li>
            <li>Basic Marketing</li>
            <li>Python for everybody</li>
            <li>Android Developer</li>
            <li>Business English</li>

        </ul>
        <ul>
            <li>Save up to 40% by paying weekly</li> 
            <li>Number of courses</li>
            <li>Time</li>
            <li>Web Designing</li>
            <li>Human-Centered Design</li>
            <li>Basic Marketing</li>
            <li>Python for everybody</li>
            <li>Android Developer</li>
            <li>Business English</li>
        </ul>

        <ul>
            <li class="active-list">Save up to 40% by paying weekly</li> 
            <li>Number of courses</li>
            <li>Time</li>
            <li>Web Designing</li>
            <li>Human-Centered Design</li>
            <li>Basic Marketing</li>
            <li>Python for everybody</li>
            <li>Android Developer</li>
            <li>Business English</li>
        </ul>

        <ul>
            <li>Save up to 40% by paying weekly</li> 
            <li>Number of courses</li>
            <li>Time</li>
            <li>Web Designing</li>
            <li>Human-Centered Design</li>
            <li>Basic Marketing</li>
            <li>Python for everybody</li>
            <li>Android Developer</li>
            <li>Business English</li>
        </ul>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
    @import '../../../style/main.scss';

    .priceTable {
        text-align: center;
        padding-top: 50px;


        &::before {
            @include backgrounds('primary');
            background-image: url('../../../assets/img/page-background-img.png');
        }

        h1 {

            color: $primary_title;
            margin-bottom:20px;
        }

        p {
            color: $primary_font;
        }

        .planTable {
            @include myflex('both');
            gap:0px;
            margin-top: 50px;

            ul:first-child li:first-child{
                
                background-color: white;
            }

            ul:nth-child(3) li:first-child.active-list {

                border-top: 3px solid $primary_color;;

            }
            
           
            ul {

            list-style: none;
            color: $primary_font;
            font-size: 0.9em;
            

                

                li {
                    width: 200px;
                    padding:20px 0px 25px 15px;
                    border: .1px solid $primary_border;
                    border-bottom: 0px;
                    border-radius: 2px;

                    &:last-child {
                        border-bottom: .1px solid $primary_border;
                        
                    }

                    &:first-child {

                        background-color: #F5FDFF;
                        border-top: 3px solid $primary_color_op;
                    }
                }
            }

        }
    }

</style>