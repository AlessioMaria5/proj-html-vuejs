<template>
  <div id="app">
    <IAccHeader/>
    <IAccMain />
    <IAccFooter />
    
    <library />
    <fas />
    <FontAwesomeIcon />
  </div>
</template>

<script>
import IAccFooter from './components/iAccFooter.vue';
import IAccHeader from './components/iAccHeader.vue';
import IAccMain from './components/iAccMain.vue';
import {library} from '@fortawesome/fontawesome-svg-core';
import {fas} from '@fortawesome/free-solid-svg-icons';
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';




export default {
  name: 'App',
  components: {
    IAccFooter,
    IAccHeader,
    IAccMain,
    fas,
    library,
    FontAwesomeIcon,
    
}
}
</script>

<style lang="scss">

</style>
