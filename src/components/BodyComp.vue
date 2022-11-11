<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col" v-for="(serie, index) in seriesArray" :key="index">
                    <img :src="serie.thumb" :alt="serie.series" class="thumb">
                    <p>{{ serie.series }}</p>
                    <!-- <p class="price">{{ serie.price }}</p> -->
                </div>

            </div>
        </div>

    </section>
</template>

<script>
import { seriesList } from '../data/series'
export default {
    name: 'BodyComp.vue',
    data() {
        return {
            seriesArray: seriesList,
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as *;
@use '../assets/styles/partials/variables' as *;

section {
    background-color: $black;
    min-height: 200px;
}

.container {
    padding: 2em 0
}

.row {
    display: flex;
    justify-content: space-between;
    flex-flow: row wrap;
    padding: 0.5em;

    .col {
        width: calc(100% / 6);
        padding: 0.7em;
    }

    img {
        width: 190px;
        height: 190px;
        object-fit: cover;
    }

    .thumb {
        object-position: 0% 0%;
    }

    p {
        padding: 0.5em 0;
        text-transform: uppercase;
    }

    .price {
        color: $lightblue;
    }
}
</style>