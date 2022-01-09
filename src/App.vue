<template>
  <app-header />
  <app-content></app-content>
  
</template>

<script>
import appHeader from './components/appHeader.vue';
import appContent from './components/appContent.vue';

export default {
  name: 'App',
  components: {
    'app-header': appHeader,
    'app-content': appContent
  }
}
</script>

<style lang="scss">
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
