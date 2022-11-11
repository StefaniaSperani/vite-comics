<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col" v-for="(serie, index) in seriesArray" :key="index">
                    <img :src="serie.thumb" alt="">
                    <p>{{ serie.series }}</p>
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
    @include dflex;
    flex-flow: row wrap;
    padding: 0.5em;
    gap: 5px;

    .col {
        width: calc(100% / 6);
    }

    img {
        width: 130px;
        height: 130px;
        object-fit: cover;
    }

    p {
        padding: 1em 0;
    }
}
</style>