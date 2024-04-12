<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';
  import {store} from './store.js'

  export default {
    components: {
      AppHeader,
      AppMain,
      AppFooter,
    },
    data(){
      return {
        store
      }
    }
  }
</script>

<template>
  <div>
    <AppHeader/>
    <AppMain/>
    <AppFooter/>
  </div>
</template>

<style lang="scss">
  @use './styles/general';
</style>