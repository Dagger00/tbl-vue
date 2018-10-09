<template>
    <section class="map" id="map">
        <div class="map__inner">
            <h3 class="map__title">К нам можно <a target="_blank" class="map__link"
                                                  href="https://yandex.ru/maps/?um=constructor%3A6c5c8306188c2d250c26c9ccf995f826fd9116b062436ab06ec083671915a2fd&source=constructorLink">приехать</a>
            </h3>
            <iframe src="https://yandex.ru/map-widget/v1/?um=constructor%3A6c5c8306188c2d250c26c9ccf995f826fd9116b062436ab06ec083671915a2fd&amp;source=constructor"
                    width="100%" height="502" frameborder="0"></iframe>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'Map',
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .map {
        margin-top: 100px;
        width: 100%;
    }

    .map__inner {
        width: 100%;
    }

    .map__title {
        width: 100%;
        text-align: center;
        font-size: 42px;
        line-height: 1.23;
    }

    .map__link {
        text-decoration: none;
        color: #ff8562;
    }

    .map__link:hover {
        border-bottom: 3px solid #ff8562;
    }
</style>
