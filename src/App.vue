<template>
  <div id="app">
    <IAccHeader/>
    <IAccMain />
    <IAccFooter />
    
  </div>
</template>

<script>
import IAccFooter from './components/iAccFooter.vue';
import IAccHeader from './components/iAccHeader.vue';
import IAccMain from './components/iAccMain.vue';




export default {
  name: 'App',
  components: {
    IAccFooter,
    IAccHeader,
    IAccMain,
    
}
}
</script>

<style lang="scss">


</style>
