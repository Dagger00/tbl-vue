<template>
    <nav class="header__nav">
        <MainOfferPhone></MainOfferPhone>
        <ul class="nav-list">
            <li class="nav-list__item"><a href="#conditions" class="nav-list__link">Условия</a></li>
            <li class="nav-list__item"><a href="#feedback" class="nav-list__link">Отзывы</a></li>
            <li class="nav-list__item"><a href="#contacts" class="nav-list__link">Контакты</a></li>
        </ul>
    </nav>
</template>

<script>
    import MainOfferPhone from './MainOfferPhone.vue'
    export default {
        name: 'Nav',
        components: {
            MainOfferPhone
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

    .nav-list {
        display: flex;
        list-style: none;
    }

    .header__nav {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .nav-list__link {
        text-decoration: none;
        color: #000000;
        margin-right: 30px;
    }

    .nav-list__link:hover {
        color: #ff8562;
    }

    @media (max-width: 570px) {

        .nav-list__link {
            text-decoration: none;
            color: #000000;
        }

    }
</style>
