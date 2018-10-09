<template>
    <section class="snow-junk-utilization" id="snow-junk-utilization">
        <div class="snow-junk-utilization__inner">
            <a class="snow-junk-utilization__button snow-junk-utilization__button_snow" href="#offer">
                <p class="snow-junk-utilization__text snow-junk-utilization__text_snow">Уборка снега</p></a>
            <a class=" snow-junk-utilization__button snow-junk-utilization__button_junk" href="#offer">
                <p class="snow-junk-utilization__text snow-junk-utilization__text_junk">Утилизация мусора</p></a>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'JunkSnow',
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .snow-junk-utilization {
        /*display: none;*/
    }

    .snow-junk-utilization__inner {
        margin: auto;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        width: 100%;
        height: 650px;
        flex-wrap: wrap;
    }

    .snow-junk-utilization__button {
        text-decoration: none;
        cursor: pointer;
        font-weight: 700;
        font-size: 30px;
        display: flex;
        justify-content: center;
        align-items: flex-end;
        height: 300px;
        width: 450px;
        background-size: cover;
        margin: 0 20px 0 20px;
    }

    .snow-junk-utilization__button:hover {
        background-size: 200%;
    }

    .snow-junk-utilization__button.snow-junk-utilization__button_snow {
        color: #000000;
        background-image: url('./../../img/snow/snow1.jpg');
        background-position: 50% 40%;
        text-shadow: -2px 0 #ffffff, 0 2px #ffffff, 2px 0 #ffffff, 0 -2px #ffffff
    }

    .snow-junk-utilization__button.snow-junk-utilization__button_junk {
        color: #ffffff;
        background-image: url('./../../img/junk/junk1.jpg');
        text-shadow: -2px 0 black, 0 2px black, 2px 0 black, 0 -2px black;
    }

    @media (max-width: 570px) {
        .snow-junk-utilization__button.snow-junk-utilization__button_snow {
            background-image: url('./../../img/snow/snow1.jpg');
            background-position: 50% 40%;
        }

        .snow-junk-utilization__button.snow-junk-utilization__button_junk {
            background-image: url('./../../img/junk/junk1.jpg');
            background-position: 33% 0%;
        }

        .snow-junk-utilization__button.snow-junk-utilization__button_snow:hover {
            background-position: 50% 40%;
            background-size: 250%;

        }

        .snow-junk-utilization__button.snow-junk-utilization__button_junk:hover {
            background-position: 33% 0%;
            background-size: 250%;

        }

    }
    .snow-junk-utilization__button.snow-junk-utilization__button_snow:hover {
        background-position: 50% 40%;
    }

    .snow-junk-utilization__button.snow-junk-utilization__button_junk:hover {
        background-position: 25% 70%;
    }

    .snow-junk-utilization__text {
        -webkit-touch-callout: none;
        -webkit-user-select: none;
        -khtml-user-select: none;
        -moz-user-select: none;
        -ms-user-select: none;
        user-select: none;
    }
</style>
