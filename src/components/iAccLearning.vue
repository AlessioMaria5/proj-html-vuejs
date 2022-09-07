<template>
  <div class="Learning">
    <GoTop />
      <div class="content-table">
        <ul>
            <!-- Acquisiti i dati degli altri elementi è possibile rendere il contenuto dinamico -->
            <li class="active-list">What We Do</li> 
            <li>Degree programme</li>
            <li>Career Achievements</li>
            <li>Personal Managment</li>
            <li>Steps to Success</li>
            <li>Knowledge Transfer</li>
        </ul>
      </div>
      <div class="content-wrap">
            <h1>Learning Possibilities</h1>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Corrupti ipsam quibusdam, in consequuntur officiis neque ducimus sunt non. Ad nobis repudiandae minima commodi odio reiciendis odit voluptates eaque. In, distinctio!</p>
        <div class="checklist-wrap">
            <ul class="checklist">
                <li><span>✓</span>We enrich lives trough learning.</li>
                <li><span>✓</span>Maximizing potential trough individual attention.</li>
                <li><span>✓</span>The trusted name for specialized training</li>
                <li><span>✓</span>People teach. People learn. This is where they connect.</li>
            </ul>
            <div class="checklist-img">
                <img src="../assets/img/h12-tabs-icon-1.png" alt="pencil with compass">
            </div>
        </div>
           
      </div>
  </div>
</template>

<script>
import GoTop from './goTop.vue';
export default {
    data() {
        return {
            iAccLearn: [
                {
                    tableTitle: "What we do",
                    sideTitle: "Learning Possibilities",
                    description: "lorem30",
                    checkList: [
                        {
                            check: "yes",
                            item: "We enrich lives through learning"
                        },
                        {
                            check: "yes",
                            item: "Maximizing potential trough individual attention."
                        },
                        {
                            check: "yes",
                            item: "The trusted name for specialized training"
                        },
                        {
                            check: "yes",
                            item: "People teach. People learn. This is where they connect."
                        }
                    ]
                }
            ]
        };
    },
    components: { GoTop }
}
</script>

<style lang="scss">
    @import '../style/main.scss';

    .Learning {
        @include myflex('hor');
        align-items: flex-end;
        padding: 50px;
        position: relative;

        .content-table {

                ul {

                    list-style: none;
                    margin-right: 20px;
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
                    }

                    .active-list {
                            border-left: 5px solid $primary_color;
                            color: $primary_color;
                            background-color: $third_bg
                            
                        }
                }
        }

        .content-wrap {
                

            
            color: $secondary_font;
            h1 {
                color: $primary_title;
                margin-bottom: 20px;
            }

            p{
                margin-bottom: 50px;
            }

            .checklist-wrap {
                @include myflex('ver');
                align-items: flex-end;
                
                .checklist {
                    width: 70%;
            
                    list-style: none;

                    li {
                        @include myflex('ver');
                        margin-bottom: 25px;
                        span {
                        color: $primary_color;
                        align-self: flex-start;
                        
                    }
                    }
                }

                .checklist-img {

                    width: 20%;
                    align-self: flex-end;
                    img {

                        width: 100%;
                    }
                }

            }
        }
    }

</style>