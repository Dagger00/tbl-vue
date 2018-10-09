<template>
    <section class="conditions" id="conditions">
        <div class="conditions__inner">
            <TechnicItem></TechnicItem>
            <TechnicItem></TechnicItem>
            <TechnicItem></TechnicItem>
        </div>
    </section>
</template>

<script>
    import TechnicItem from './TechnicItem.vue'
    export default {
        name: 'Conditions',
        components: {
            TechnicItem,
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .conditions__inner {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        margin: auto;
        margin-top: 80px;
        padding-bottom: 120px;
    }
</style>
