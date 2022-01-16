<template lang="">
    <div class="contentArea">
        <content-about></content-about>
        <content-project></content-project>
        <content-contact></content-contact>
    </div>
</template>
<script>
import ContentAbout from './ContentAbout.vue';
import ContentContact from './ContentContact.vue';
import ContentProject from './ContentProject.vue';

export default {
    name: 'appContent',
    components: {
        'content-about': ContentAbout,
        'content-contact': ContentContact,
        'content-project': ContentProject
    }
}
</script>
<style lang="scss">
@import '../scss/Container.scss';
</style>