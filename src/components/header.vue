<template>
    <header class="header">
        <div class="header__inner">
            <Logo></Logo>
            <Nav></Nav>
        </div>
    </header>
</template>

<script>
    import Logo from './Logo.vue'
    import Nav from './Nav.vue'

    export default {
        name: 'Header',
        components: {
            Logo,
            Nav
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .header {
        font-size: 24px;
        margin: auto;
    }
    .header__inner {
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
    }

    @media (max-width: 570px) {

        .header {
            font-size: 18px;
            margin: auto;
        }
    }

</style>
