<template>
    <section class="feedback" id="feedback">
        <div class="feedback__inner">
            <h2 class="feedback__title">Отзывы наших клиентов</h2>
            <div class="feedback__items">
                <div class="feedback__item feedback__item_active">
                    <p class="feedback__text"><!--{{feedback.f1.text}}--></p>
                    <div class="feedback__photo feedback__photo_1"></div>
                    <p class="feedback__name"><!--{{feedback.f1.name}}--></p>
                </div>
                <div class="feedback__item">
                    <p class="feedback__text"><!--{{feedback.f2.text}}--></p>
                    <div class="feedback__photo feedback__photo_2"></div>
                    <p class="feedback__name"><!--{{feedback.f2.name}}--></p>
                </div>
                <div class="feedback__item">
                    <p class="feedback__text"><!--{{feedback.f3.text}}--></p>
                    <div class="feedback__photo feedback__photo_3"></div>
                    <p class="feedback__name"><!--{{feedback.f3.name}}--></p>
                </div>
            </div>
            <div class="feedback__dots">
                <div class="feedback__dot feedback__dot_active"></div>
                <div class="feedback__dot"></div>
                <div class="feedback__dot"></div>
            </div>

            <div class="feedback__buttons-container">

                <div class="feedback__button-container feedback__button-container_left" onclick="plusSlides(-1)">
                    <div class="feedback__mini-container feedback__mini-container_left">
                        <div class="feedback__button feedback__button_left"></div>
                    </div>
                </div>
                <div class="feedback__button-container feedback__button-container_right" onclick="plusSlides(1)">
                    <div class="feedback__mini-container feedback__mini-container_right">
                        <div class="feedback__button feedback__button_right"></div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'Feedback'
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .feedback {
        height: 700px;
        background-color: #ebebeb;
        width: 100%;
    }

    .feedback__inner {
        display: flex;
        justify-content: center;
        flex-direction: column;
        margin: auto;
        text-align: center;
        padding: 120px 0 0 0;
    }

    .feedback__title {
        font-size: 42px;
        line-height: 1.23;
    }

    .feedback__items {
        padding-top: 20px;
    }

    .feedback__item {
        display: none;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        max-width: 700px;
        margin: auto;
    }

    .feedback__item.feedback__item_active {
        display: flex;
    }

    .feedback__text {
        font-size: 22px;
        line-height: 1.55;
        font-weight: 300;
    }

    .feedback__name {
        font-size: 16px;
        line-height: 1.35;
        font-weight: 600;
    }

    .feedback__photo {
        width: 100px;
        height: 100px;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        border-radius: 50%;
    }

    .feedback__photo_1 {
        background-image: url("./../../img/otziv-1.jpg");
    }

    .feedback__photo_2 {
        background-image: url("./../../img/otziv-2.jpeg");
    }

    .feedback__photo_3 {
        background-image: url("./../../img/otziv-3.jpeg");
    }

    .feedback__buttons-container {
        position: relative;
    }

    .feedback__button-container {
        position: absolute;
        height: 278px;
        cursor: pointer;
        z-index: 4;
        box-sizing: content-box;
        bottom: 0;
        width: 15%;
        -webkit-transition: opacity ease-in-out 0.3s, height ease-in-out .3s;
        -moz-transition: opacity ease-in-out 0.3s, height ease-in-out .3s;
        -o-transition: opacity ease-in-out 0.3s, height ease-in-out .3s;
        transition: opacity ease-in-out 0.3s, height ease-in-out .3s;
    }

    .feedback__button-container_left {
        left: 0;
    }

    .feedback__button-container_right {
        right: 0;
    }

    .feedback__mini-container {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
    }

    .feedback__mini-container_left {
        left: 30px;
    }

    .feedback__mini-container_right {
        right: 30px;
    }

    .feedback__button {
        position: absolute;
        width: 20px;
        height: 20px;
        transform: rotate(45deg);
        background: transparent;
        box-sizing: content-box;
        cursor: pointer;
    }

    .feedback__button_left {
        border-bottom: 1px solid;
        border-left: 1px solid;
        border-color: #ff5c33;
    }

    .feedback__button_right {
        border-top: 1px solid;
        border-right: 1px solid;
        border-color: #ff5c33;
    }

    .feedback__dots {
        display: flex;
        justify-content: center;
    }

    .feedback__dot {
        cursor: pointer;
        margin: 0 5px;
        width: 5px;
        height: 5px;
        background-color: #ff5c33;
        border-radius: 10px;
        opacity: .4;
    }

    .feedback__dot_active {
        opacity: 1;
    }

    @media (max-width: 570px) {
        .feedback__inner {
            padding: 0 0 0 0;
        }

        .feedback__title {
            margin: 20px 0 0 0;
        }

        .feedback__items {
            padding: 0 0 0 0;
        }

    }
</style>
