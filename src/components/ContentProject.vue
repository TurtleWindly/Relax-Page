<template>
    <div class="wave-project">
        <h2>Project</h2>
            <div class="projects">
                <div class="comming-now">
                    <div class="inkscape"><img src="../assets/pirate_gun_polygons.png" alt="pirate_gun_polygons"></div>
                    <div class="description">Pirate gun polygons</div>
                </div>
                <div class="comming-soon"><p>Comming soon</p></div>
                <div class="comming-soon"><p>Comming soon</p></div>
            </div>
    </div>
  
</template>

<script>
export default {
    name:'ContentProject'
}
</script>

<style lang="scss" scoped>
    .wave-project {
        transition: 1s all;
        aspect-ratio: 960/540;
        width: 100%;
        height: auto;
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        background-image: url(../assets/waveFooterD.svg);
        position: relative;
        top: 0;
        @media screen and (max-width: 635px){
            aspect-ratio: 960/960;
        }
    }
    .comming-now, .comming-soon {
        transition: 1s all;
        width: 200px;
        height: 100px;
        background-color: #4dc8e6;
        border-radius: 15px;
        @media screen and (max-width: 635px){
            width: 150px;
            height: 75px;
            font-size: 0.7em;
        }
    }
    .comming-now {
        .inkscape {
            width: 100%;
            height: 80%;
            display: flex;
            justify-content: center;
            align-items: center;
            img {
                height: 90%;
                width: 90%;
            }
        }
        .description {
            height: 20%;
            background-color: #3668c8;
            border-radius: 0 0 15px 15px;
            text-align: center;
        }
    }
    .comming-soon {
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 1.2em;
    }
    .projects {
        transition: 1s all;
        color: white;
        display: flex;
        justify-content: space-around;
        margin: 50px 0 0 0;
        @media screen and (max-width: 635px){
            margin: 25px 0 0 0;
            flex-direction: column;
            align-items: center;
            .comming-now, .comming-soon {
                margin-bottom: 5px;
            }
        }
        @media screen and (min-width: 1200px){
            margin: 150px 0 0 0;
        }
    }
</style>