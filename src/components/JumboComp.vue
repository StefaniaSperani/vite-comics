<template>
    <div class="jumbo">
        <button class="series">Current Series</button>
    </div>

</template>

<script>
export default {
    name: 'JumboComp',
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as *;
@use '../assets/styles/partials/variables' as *;

.jumbo {
    background-image: url(../assets/img/jumbotron.jpg);
    min-height: 400px;
    position: relative;
}

.series {
    text-transform: uppercase;
    padding: 13px;
    background-color: $lightblue;
    font-weight: bold;
    color: #fff;
    border: none;
    font-size: 1.2em;
    position: absolute;
    bottom: -25px;
    left: 300px;
}
</style>