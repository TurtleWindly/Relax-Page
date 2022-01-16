<template lang="">
        <transition appear name="fade" 
          @before-enter="beforeEnter" 
          @enter="enter"
          @before-leave="beforeLeave"
          @leave="leave"
        >
            <div v-if="loadingTime" class="wave"></div>
        </transition>
</template>
<script>
import gsap from "gsap";

export default {
  name: "LoaderScreen",
  data() {
    return {
      loadingTime: true
    };
  },
  mounted() {
    setTimeout(() => {
      this.loadingTime = false
      clearTimeout(this.setTimeout);
    }, 5000);
  },
  methods: {
    beforeEnter(el) {
        el.style.opacity = 0
        console.log(1)
    },
    enter(el){
        console.log(2)
        gsap.to(el, {
            opacity: 1,
            duration: 2
        })
    },
      beforeLeave(el){
        console.log(3)
        el.style.opacity = 1
      },
    leave(el){
      console.log(4)
      gsap.to(el,{
        opacity: 0,
        duration: 2
      })
      },

  },
};
</script>
<style lang="scss">
@import "../scss/loadingScreen";
body.disabled {
    overflow-x: hidden; //horizontal
    overflow-y: hidden; //vertical
}
</style>