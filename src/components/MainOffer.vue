<template>
    <section class="main-offer" id="offer">
        <div class="main-offer__inner">
            <h2 class="main-offer__title"><!--{{mainOffer}}--></h2>
            <p class="main-offer__description main-offer__description_star">*Цена рассчитывается индивидуально</p>

            <div class="main-offer__info">
                <div class="main-offer__text">
                    <p class="main-offer__description">Позвоните</p>

                    <a href="tel:+74951426238" class="main-offer__phone">+7(495)142-62-38</a>
                    <p class="main-offer__description">Или оставьте свои контакты</p>
                </div>
                <form class="main-offer__form" action="https://formspree.io/info@tobelease.ru" method="post">
                    <input type="hidden" name="_next" value="https://tobelease.ru/#thankyou"/>
                    <input type="hidden" name="_subject" value="Заявка с сайта tobelease.ru"/>
                    <StandartInput></StandartInput>
                    <StandartInput></StandartInput>
                    <input type="hidden" name="_language" value="ru"/>
                    <button class="contacts__button" type="submit">Позвоните мне</button>
                </form>
            </div>
        </div>
    </section>
</template>

<script>
    import StandartInput from './StandartInput.vue'

    export default {
        name: 'MainOffer',
        components: {
            StandartInput
        }

    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .main-offer {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    .main-offer__inner {
        display: flex;
        flex-direction: column;
        justify-content: center;
        margin: auto;
        margin-top: 100px;
    }

    .main-offer__title {
        text-align: center;
        font-size: 64px;
        font-weight: 700;
        line-height: 1.23;
        margin-bottom: 10px;
    }

    .main-offer__text {
        text-align: center;
        font-weight: 300;
        font-size: 24px;
        color: #8a8a8a;
    }

    .main-offer__form {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .main-offer__phone {
        color: #ff8562;
        text-decoration: none;
        font-size: 30px;
        line-height: 1.45;
    }

    .main-offer__description_star {
        margin: 0 0 20px 0;
        align-self: center;
        color: #8a8a8a;
    }

    @media (max-width: 570px) {

        .main-offer__title {
            font-size: 32px;
        }
    }
</style>
