<template>
    <div>
        <div class="conditions__image conditions__image_num_1 image" v-bind:style="{ backgroundImage: 'url(' + imgSrc + ')' }"></div>
        <img class="image1" v-bind:src="imgSrc" alt="" style="display: none">
    </div>
</template>

<script>
    export default {
        name: 'TechnicImage',
        props: {imgSrc: String}
    }
</script>

<style scoped>
    .conditions__image {
        cursor: pointer;
        width: 450px;
        height: 450px;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
    }
</style>