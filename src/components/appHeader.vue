<template>
  <header>
    <nav-header></nav-header>
    <div id="background"></div>
  </header>
    
</template>

<script>
import navHeader from '@/components/navHeader.vue'

export default {
  name: 'appHeader',
  components: {
    'nav-header': navHeader
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
  @import '../scss/appHeader';
</style>
