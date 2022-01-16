<template lang="">
    <nav>
        <img src="../assets/relax_logo.png" alt="relax logo">
        <h1>Relax Studio</h1>
       <ul>
           <li @click="scrollToAbout">About</li>
           <li @click="scrollToProject">Project</li>
           <li @click="scrollToContact">Contact</li>
       </ul> 
    </nav>
</template>
<script>
export default {
    name: 'navHeader',
    methods: {
        scrollTo(id) {
            // document.getElementById('About').scrollIntoView({behavior: 'smooth', block: 'start'})
            const about = document.getElementById(id)
            let position = about.getBoundingClientRect()
            // position.left, position.top + window.scrollY - 90,
            window.scroll({
                behavior: 'smooth',
                top: (position.left, position.top + window.scrollY - 90),
            })
        },
        scrollToAbout() {
            this.scrollTo('About')
        },
        scrollToProject() {
            this.scrollTo('Project')
        },
        scrollToContact() {
            this.scrollTo('Contact')
        }
    }
}
</script>
<style lang="scss" scoped>
    li:hover {
        cursor: pointer;
    }
</style>