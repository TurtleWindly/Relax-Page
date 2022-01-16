<template>
    <footer>
        <h2>Contact</h2>
        <ul>
            <li>
                <img src="../assets/email_icon.jpg" alt="email">
                <p>relax.companii@gmail.com</p>
            </li>
            <li>
                <img src="../assets/facebook_icon.jpg" alt="facebook">
                <p>This is my personal account but don't have anythings special yet</p>
            </li>
            <li>
                <a href="https://github.com/TurtleWindly">
                    <img src="../assets/github_icon.jpg" alt="github">
                    <p>And this is special where I put my code on and some small project with also have my first web page</p>
                </a>
            </li>
        </ul>
    </footer>
</template>

<script>
export default {
    name: 'ContentContact',
}
</script>

<style lang="scss" scoped>
    footer {
        /* svg background */
        z-index: 200;
        aspect-ratio: 960/540;
        width: 100%;
        height: 50vh;
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        background-image: url(../assets/buble.svg);
        top: 0;
        @media screen and (max-width: 635px){
            height: 50vh
        }
        // color things
        color: white;
    }
    @mixin flex-center {
        display: flex;
        align-items: center;
    }
    li {
        @include flex-center;
        list-style: none;
        a {
            display: flex;
            align-items: center;
            text-decoration: none;
        }
        img {
            width: 30px;
            height: 30px;
            margin-right: 5px;
        }
    }
    
</style>