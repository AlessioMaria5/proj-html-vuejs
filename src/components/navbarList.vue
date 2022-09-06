<template>
  <div id="navbarList">
      <ul>
          <a v-for="(singleLink,index) in nav" :key="index" :href="singleLink.link"><li>{{singleLink.name}}</li></a>
      </ul>
  </div>
</template>

<script>
export default {

    name: 'navbarList',
    data() {
        return {

            nav:[
                {
                    name: 'Home',
                    link: '#'
                },

                {
                    name: 'Courses',
                    link: '#'
                },

                {
                    name: 'Instructors',
                    link: '#'
                },

                {
                    name: 'Events',
                    link: '#'
                },

                {
                    name: 'Pages',
                    link: '#'
                },

                {
                    name: 'Elements',
                    link: '#'
                },

                ]

        }
    }

}
</script>

<style lang="scss" scoped>

@import '../style/main.scss';

#navbarList {

    ul {

        @include myflex('ver');
        
    }
}
</style>