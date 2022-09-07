<template>
  <div class="priceTable">
    <h1>Pricing Plans</h1>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Velit</p>

      <div class="planTable">
        <ul>
            <li>
                <h2>Save up to 40% by paying weekly</h2> 
            </li> 
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
            <li>
                <div class="course-icon-wrap">
                    <img src="../../../assets/img/h5-custom-icon-7.png" alt="">
                </div>
                <h2>Standard</h2> 
                <div class="price">$12</div>
            </li> 
            <li>2</li>
            <li>15 Days</li>
            <li>Web Designing</li>
            <li>Human-Centered Design</li>
            <li>Basic Marketing</li>
            <li>Python for everybody</li>
            <li>Android Developer</li>
            <li>Business English</li>
            <li class="list-btn"><a href="#">GET IT KNOW</a></li>
        </ul>

        <ul>
            <li class="active-list">
                <div class="course-icon-wrap">
                    <img src="../../../assets/img/h5-custom-icon-8.png" alt="">
                </div>
                <h2>Professional</h2>
                <div class="price">$59</div>
            </li> 
            <li>4</li>
            <li>30 Days</li>
            <li>Web Designing</li>
            <li>Human-Centered Design</li>
            <li>Basic Marketing</li>
            <li>Python for everybody</li>
            <li>Android Developer</li>
            <li>Business English</li>
            <li class="list-btn"><a href="#">GET IT KNOW</a></li>
        </ul>

        <ul>
            <li>
                <div class="course-icon-wrap">
                    <img src="../../../assets/img/h5-custom-icon-9.png" alt="">
                </div>
                <h2>Advanced</h2>
                <div class="price">$88</div> 
            </li>  
            <li>6</li>
            <li>30 Days</li>
            <li>Web Designing</li>
            <li>Human-Centered Design</li>
            <li>Basic Marketing</li>
            <li>Python for everybody</li>
            <li>Android Developer</li>
            <li>Business English</li>
            <li class="list-btn"><a href="#">GET IT KNOW</a></li>
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
    @import '../../../style/buttons.scss';

    .priceTable {
        text-align: center;
        padding-top: 50px;
        padding-bottom: 50px;


        &::before {
            
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
                text-align: start;
            }

            ul:first-child {
                align-self: flex-start;
            }


            ul:nth-child(3) {
                a {
                    @include styleBtn('classic')
                }
                li:first-child.active-list {
                border-top: 3px solid $primary_color;
            }
            }
            
            
           
            ul {

            list-style: none;
            color: $primary_font;
            font-size: 0.9em;

            .list-btn {

                background-color: $secondary_bg;
            }

            a {
                    @include styleBtn('secondary');
                }
            

                

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
                        height: 200px;
                        display: flex;
                        flex-direction:column;
                        justify-content: end;
                        padding: 20px;

                        .course-icon-wrap {

                            width: 100%;

                            img {
                                width: 50%;
                                margin-bottom: 20px;
                            }
                        }
                    }
                }
            }

        }
    }

</style>