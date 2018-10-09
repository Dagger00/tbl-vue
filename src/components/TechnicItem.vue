<template>
    <div class="conditions__item">
        <TechnicImage v-bind:imgSrc="imgSrc"></TechnicImage>
        <h2 class="conditions__title">Кран-манипулятор</h2>
        <TechnicDescription v-bind:escriptionObject="descriptionObject"></TechnicDescription>
        <TechnicButton></TechnicButton>
    </div>
</template>

<script>
    import TechnicImage from './TechnicImage.vue'
    import TechnicDescription from './TechnicDescription.vue'
    import TechnicButton from './TechnicButton.vue'
    export default {
        name: 'TechnicItem',
        components: {
            TechnicImage,
            TechnicDescription,
            TechnicButton
        },
        props: {
            imgSrc: String,
            descriptionObject: Object,
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .conditions__item {
        max-width: 450px;
        display: flex;
        flex-direction: column;
        margin: 20px;
        box-sizing: border-box;
    }

    .conditions__image {
        cursor: pointer;
        width: 450px;
        height: 450px;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
    }

    .conditions__title {
        text-align: center;
        padding: 0;
        margin: 0;
        margin-top: 15px;
    }
</style>
