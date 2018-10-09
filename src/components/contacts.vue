<template>
    <section class="contacts" id="contacts">
        <div class="contacts__inner">
            <h2 class="contacts__title">Остались вопросы?</h2>
            <div class="contacts__info">
                <div class="contacts__text">
                    <p class="contacts__field contacts__phone">Телефон:<br><a href="tel:+74951426238"
                                                                              class="main-offer__phone">+7(495)142-62-38</a>
                    </p>
                    <p class="contacts__field contacts__email">Почта:<br> <a class="contacts__link"
                                                                             href="mailto:hello@firm.com">info@tobelease.ru </a>
                    </p>
                    <p class="contacts__field contacts__address">Московская область, Солнечногорский район, сельское
                        поселение Кутузовское, д. Голиково, д. 103</p>
                </div>
                <form class="contacts__form" action="https://formspree.io/info@tobelease.ru" method="post">
                    <input type="hidden" name="_next" value="https://tobelease.ru/#thankyou"/>
                    <input type="hidden" name="_subject" value="Заявка с сайта tobelease.ru"/>
                    <StandartInput></StandartInput>
                    <StandartInput></StandartInput>
                    <StandartInput></StandartInput>
                    <input type="hidden" name="_language" value="ru"/>
                    <button class="contacts__button" type="submit">Отправить</button>
                </form>
            </div>
        </div>
    </section>
</template>

<script>
    import StandartInput from './StandartInput.vue'
    export default {
        name: 'Contacts',
        components: {
            StandartInput
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .contacts__inner {
        max-width: 1200px;
        margin: auto;
        padding-top: 100px;
        padding-bottom: 100px;
    }

    .contacts__title {
        width: 100%;
        text-align: center;
        font-size: 42px;
        line-height: 1.23;
    }

    .contacts__info {
        display: flex;
        flex-wrap: wrap;
    }

    .contacts__info > * {
        margin-left: 50px;
        margin-right: 50px;
        font-weight: 300;
    }

    .contacts__text {
        padding: 0 50px 0 50px;
        max-width: 436px;
    }

    .contacts__phone {
        font-size: 30px;
        line-height: 1.45;
    }

    .contacts__phone > a {
        color: #ff8562;
        font-size: 30px;
        line-height: 1.45;
    }

    .contacts__email {
        font-size: 30px;
        line-height: 1.45;
    }

    .contacts__link {
        color: #ff8562;
        text-decoration: none;
    }

    .contacts__address {
        font-size: 18px;
        line-height: 1.55;
        font-weight: 300;
    }

    .contacts__form {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .contacts__input {
        text-align: center;
        font-size: 20px;
        margin-top: 25px;
        border: none;
        background-color: #f2f2f2;
        height: 60px;
        width: 460px;
    }

    .contacts__input.contacts__input_textarea {
        height: 80px;
    }

    .contacts__button {
        margin-top: 30px;
        background-color: #eb633d;
        border: none;
        width: 300px;
        height: 60px;
        border-bottom-left-radius: 6px;
        border-bottom-right-radius: 6px;
        border-top-right-radius: 6px;
        border-top-left-radius: 6px;
        cursor: pointer;
        font-weight: 700;
        color: #ffffff;
    }

    @media (max-width: 980px) {
        .contacts__info {
            flex-direction: column;
        }

    }

    @media (max-width: 570px) {
        .contacts__inner {
            max-width: 350px;
        }

        .contacts__field {
            margin: 20px 10px 0 3px;
        }

        .contacts__text {
            display: flex;
            flex-direction: column;
            padding: 0 0 0 0;
            width: 100%;
            align-items: flex-start;
            justify-content: center;
            text-align: justify;

        }

        .contacts__input {
            width: 310px;
        }

        .contacts__info > * {
            margin-left: 0;
            margin-right: 0;
        }

    }
</style>
