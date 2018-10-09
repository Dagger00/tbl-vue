<template>
    <ul class="description description1">
        <li class="description__item"><span>Вылет стрелы</span> <span>12, 16, 18, 22 м.</span></li>
        <li class="description__item"><span>Грузоподъемность кузова</span> <span>3-20 т.</span></li>
        <li class="description__item"><span>Грузоподъемность стрелы</span> <span>2-25 т.</span></li>
        <li class="description__item"><span>Длина кузова</span> <span>3-12 м.</span></li>
        <li class="description__item"><span>Тип проходимости:</span> <span>колесный</span></li>
        <li class="description__item"><span>Ширина кузова</span> <span>2,35 - 2,5 м.</span></li>
        <li class="description__item"><span>Цена</span> <span>1000-1500 руб./ч.</span></li>
    </ul>
</template>

<script>
    export default {
        name: 'TechnicDescription',
    }
</script>

<style scoped>
    .description {
        margin: auto;
        position: relative;
        list-style: none;
        padding: 0;
        min-height: 90px;
        width: 362px;
    }

    .description__item {
        position: relative;
        line-height: 25px;
    }

    .description__item span:nth-child(n) {
        display: inline-block;
        background: #fff;
        position: relative;
        padding: 0 3px;
        font-weight: 300;
    }

    .description__item span:nth-child(2n) {
        font-weight: 500;
        float: right;
        width: 115px;
        text-align: left;
        display: inline-block;
        background: #fff;
        position: relative;
        padding: 0 3px;
        white-space: nowrap;
    }

    .description__item::before {
        border-bottom: 1px solid #ebebeb;
        display: inline-block;
        content: '';
        width: 100%;
        position: absolute;
        bottom: 7px;
        box-sizing: border-box;
    }
</style>