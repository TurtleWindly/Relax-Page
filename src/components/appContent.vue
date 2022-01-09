<template lang="">
    <div class="contentArea">
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Id eum ea quidem? A culpa quaerat temporibus fuga tenetur facilis libero, reiciendis recusandae tempore dolor, quod repellendus alias, rem odio cupiditate!</p>
    </div>
</template>
<script>
export default {
    name: 'appContent'
}
</script>
<style lang="scss">
.contentArea {
    margin-top: 30px;
    width: 100%;
    position: relative;
    top: 370px;
    background: #fff;
    height: auto;
}

@media screen and (max-width: 635px) {
    .contentArea {
        top: 270px;
    }
}
</style>