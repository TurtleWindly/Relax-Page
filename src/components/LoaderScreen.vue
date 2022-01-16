<template lang="">
        <div class="trinity-rings-spinner" v-if="isLoad">
          <div class="circle"></div>
          <div class="circle"></div>
          <div class="circle"></div>
        </div>
</template>
<script>

export default {
  name: "LoaderScreen",
  data() {
    return {
      isLoad: true
    };
  },
  mounted() {
    document.body.style.overflow = "hidden";
    setTimeout(() => {
      this.isLoad= false
      document.body.style.overflow = "visible";
      clearTimeout(this.setTimeout);
    }, 2000);
  },
};
</script>
<style lang="scss">
@import "../scss/loadingScreen";
</style>