<template>
    <section class="how" id="how">
        <div class="how__inner">
            <h2 class="how__title">Как мы работаем?</h2>
            <div class="how__container">
                <div class="how__item">
                    <img src="./../../img/icons/noun_Phone_1701531.png" alt="" class="how__img">
                    <p class="how__text">
                        <a class="how__b_orange" href="#offer">Звоните</a> или <a class="how__b_orange" href="#offer">Оставляете
                        заявку</a>
                    </p>
                </div>
                <div class="how__item">
                    <img src="./../../img/icons/noun_dialog_332789.png" alt="" class="how__img">
                    <p class="how__text">
                        <b>Обсуждаем детали</b>
                    </p>
                </div>
                <div class="how__item">
                    <img src="./../../img/icons/noun_Ruble Wallet.png" alt="" class="how__img">
                    <p class="how__text">
                        <b>Договариваемся об условиях оплаты</b>
                    </p>
                </div>
                <div class="how__item">
                    <img src="./../../img/icons/crane.png" alt="" class="how__img">
                    <p class="how__text">
                        <b>Принимаете технику</b>
                    </p>
                </div>
                <div class="how__item">
                    <img src="./../../img/icons/noun_Document_745677.png" alt="" class="how__img">
                    <p class="how__text">
                        <b>Предоставляем отчётные документы</b>
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'HowWorks'
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .how {
        width: 100%;
    }

    .how__inner {
        width: 90%;
        margin: auto;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-bottom: 100px;
    }

    .how__title {
        text-align: center;
        font-size: 48px;
        font-weight: 700;
        line-height: 1.23;
    }

    .how__container {
        font-size: 19px;
        width: 100%;
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
    }

    .how__item {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .how__img {
        width: 70px;
        height: 70px;
        border-radius: 10%;
        margin-top: 40px;
        fill: black;

    }

    .how__img.how__img_long {
        width: 70px;
        height: 60px;
    }

    .how__text {
        max-width: 200px;
        text-align: center;
    }

    .how__b_orange {
        color: #eb633d;
        cursor: pointer;
        font-weight: bold;
        text-decoration: none;
    }
</style>
