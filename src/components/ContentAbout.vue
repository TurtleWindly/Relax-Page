<template lang="">
    <div>
        <h2>About</h2>
        <div class="para" v-for="(detail, index) in details" :key="index">
            <div>
                <img :src="detail.icon">
                <p>{{detail.text}}</p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'ContentAbout',
    data() {
        return {
            details: [
                {icon: require('../assets/turtle_icon.png'), text: 'I am student with free time and a laptop on a journey to    explore The Internet. I make projects for fun and improve my skill in programming, web development, game development'},
                {icon: require('../assets/godot_icon.png'), text: 'At the time I create this page I am using Godot to make game but it have been delay cause... creating this page'},
                {icon: require('../assets/sass_logo.png'), text: 'I also learning orther things like css with superpower! Sass! All my nightmares were gone because Sass is my hero'},
                {icon: require('../assets/js_icon.png'), text: 'In my roadmap I also try to use framework. And now I know vanila javascript is madness to use in a web application'},
                {icon: require('../assets/vue_logo.png'), text: 'My framework is Vue and it so awsome! I never want to go back vanila javascript anymore. But I am still new so I decide practice more by making projects'},
                {icon: require('../assets/java_icon.png'), text: 'I also know Java. My favorite programming language but i don\'t use it very much'},
                {icon: require('../assets/Cpp_icon.png'), text: 'And my programming skill finally up to intermediate after self-learning for 2 years cause I learn on a very good website that I will never forget. But it taught C++ so I can use C++ too'},
                {icon: require('../assets/inkscape_icon.png'), text: 'Too keep every things wonderful and my eye not exploded I have created my own logo. And some cool art with Inkscape - A free graphic design open source software'},
            ]
        }
    },
}

</script>
<style lang="scss" scoped>
.para {
    div {
        display: flex;
        align-items: center;
        img {
            width: 30px;
            height: 30px;
            margin-right: 5px;
        }
    }

}
</style>