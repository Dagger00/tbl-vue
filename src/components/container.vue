<template>
    <div class="container">
        <Offer></Offer>
        <JunkSnow></JunkSnow>
        <conditions></conditions>
        <HowWorks></HowWorks>
        <WhyWe></WhyWe>
        <feedback></feedback>
        <MainOffer></MainOffer>
        <Map></Map>
        <contacts></contacts>
    </div>
</template>

<script>
    import Offer from './Offer.vue'
    import JunkSnow from './JunkSnow.vue'
    import conditions from './conditions.vue'
    import HowWorks from './how-works.vue'
    import WhyWe from './WhyWe.vue'
    import feedback from './feedback.vue'
    import MainOffer from './MainOffer.vue'
    import Map from './Map.vue'
    import contacts from './contacts.vue'
    export default {
        name: 'container',
        components: {
            Offer,
            JunkSnow,
            conditions,
            HowWorks,
            WhyWe,
            feedback,
            MainOffer,
            Map,
            contacts
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .container {
        background-color: #ffffff;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
</style>
