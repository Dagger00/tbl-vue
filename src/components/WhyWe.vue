<template>
    <section class="why" id="why">
        <div class="why__inner">
            <h2 class="why__title">Почему мы?</h2>
            <div class="why__container">
                <div class="why__item">
                    <img src="./../../img/icons/noun_Money_1881640.png" alt="" class="why__img">
                    <p class="why__text">
                        <b>Самая</b> низкая цена на аренду спецтехники
                    </p>
                </div>
                <div class="why__item">
                    <img src="./../../img/icons/noun_Percent2.png" alt="" class="why__img">
                    <p class="why__text">
                        При заказе от 30 смен обратная доставка за <b>наш счет</b>
                    </p>
                </div>
                <div class="why__item">
                    <img src="./../../img/icons/Kremlin.png" alt="" class="why__img">
                    <p class="why__text">
                        <b>Пропуска</b> в центр Москвы
                    </p>
                </div>
                <div class="why__item">
                    <img src="./../../img/icons/logo-rst.png" alt="" class="why__img why__img_long">
                    <p class="why__text">
                        <b>Разрешение</b> от Ростехнадзора
                    </p>
                </div>
                <div class="why__item">
                    <img src="./../../img/icons/debit card.png" alt="" class="why__img">
                    <p class="why__text">
                        <b>Рассрочка</b> от Банков-партнёров
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'WhyWe'
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .why {
        width: 100%;
    }

    .why__inner {
        width: 90%;
        margin: auto;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-bottom: 100px;
    }

    .why__title {
        text-align: center;
        font-size: 48px;
        font-weight: 700;
        line-height: 1.23;
    }

    .why__container {
        font-size: 19px;
        width: 100%;
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
    }

    .why__item {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .why__img {
        width: 70px;
        height: 70px;
        border-radius: 10%;
        margin-top: 40px;
    }

    .why__img.why__img_long {
        width: 70px;
        height: 60px;
    }

    .why__text {
        max-width: 200px;
        text-align: center;
    }
</style>
