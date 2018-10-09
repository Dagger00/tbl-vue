<template>
    <section class="offer">
        <div class="offer__inner">
            <h1 class="offer__title"><!--{{offerTitle}}-->ХУЙ??</h1>
            <p class="offer__text">Собственный автопарк и сотни партнёров.</p>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'Offer',
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .offer {
        display: flex;
        align-items: center;
        align-self: flex-start;
        margin-left: 220px;
    }

    .offer__inner {
        max-width: 760px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        margin-left: 20%;
        margin-top: 100px;
    }

    .offer__title {
        font-size: 64px;
        font-weight: 700;
        line-height: 1.23;
        text-align: left;
    }

    .offer__text {
        font-weight: 300;
        font-size: 20px;
        text-align: left;
        color: #8a8a8a;
    }

    @media (max-width: 1200px) {
        .offer__inner {
            margin-left: 5%;
        }

        .offer {
            margin-left: 0;
            align-self: center;
        }

    }

    @media (max-width: 570px) {
        .offer__title {
            font-size: 48px;
            text-align: center;
        }

        .offer__text {
            font-size: 20px;
            text-align: center;
        }

        .offer__inner {
            margin-left: 5%;
        }

        .offer {
            margin-left: 0;
            align-self: center;
        }

    }
</style>
