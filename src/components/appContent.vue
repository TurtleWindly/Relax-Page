<template lang="">
    <div class="contentArea">
        <content-about></content-about>
        <content-contact></content-contact>
    </div>
</template>
<script>
import ContentAbout from './ContentAbout.vue';
import ContentContact from './ContentContact.vue';

export default {
    name: 'appContent',
    components: {
        'content-about': ContentAbout,
        'content-contact': ContentContact
    }
}
</script>
<style lang="scss">
@import '../scss/Container.scss';
</style>