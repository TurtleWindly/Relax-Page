<template>
  
  <app-header></app-header>
  <app-content></app-content>
  <loader-screen></loader-screen>

</template>

<script>
import appHeader from './components/appHeader.vue';
import appContent from './components/appContent.vue';
import LoaderScreen from './components/LoaderScreen.vue';

export default {
  name: 'App',
  components: {
    'app-header': appHeader,
    'app-content': appContent,
    'loader-screen': LoaderScreen
  },
}
</script>

<style lang="scss">
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}


</style>
