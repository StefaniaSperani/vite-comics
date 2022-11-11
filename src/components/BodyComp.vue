<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col">
                    <img src="../assets/img/dc-logo.png" alt="">
                    <p>Action comics</p>
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
    },
    mounted() {
        console.log(this.seriesArray);
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

.row {
    @include dflex;
    flex-flow: row wrap;

    .col {
        width: calc(100% / 6);
        padding: 2rem;
    }
}
</style>