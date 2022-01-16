<template lang="">
    <div class="contentArea">
        <content-about id="About"></content-about>
        <content-project id="Project"></content-project>
        <content-contact id="Contact"></content-contact>
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