<template>
  <div class="navbar">
      <div class="logo"><img src="../assets/img/logo-light.png" alt=""></div>
      <NavbarList />
      <div class="eShop">
          <ul>
              <a href="#"><li>X</li></a>
              <a href="#"><li>X</li></a>
              <a href="#"><li>X</li></a>
          </ul>
      </div>
  </div>
</template>

<script>
import NavbarList from './navbarList.vue';
// import { library } from '@fortawesome/fontawesome-svg-core'

export default {
    components: { NavbarList}
}
</script>


<style lang="scss">

    @import '../style/main.scss';

    .navbar {        
        
        @include myflex('both');
        justify-content: space-between;
        padding: 5px 20px;

        ul {

           li , a {
            @include navList('noStyle');
            color:White;
            text-transform:uppercase;
            font-size: 0.8em;
            font-weight: 100;
        }
        }

        .eShop {

            ul {

                @include myflex('both');
            }
        }
        
    }
    .logo {
         img {
             width:150px;
         }
    }

    

</style>