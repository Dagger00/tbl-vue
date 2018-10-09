<template>
    <label>
        <input name="name" class="contacts__input" data-type="text" placeholder="Иван Иванович">
    </label>
</template>

<script>
    export default {
        name: 'Input',
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
</style>
