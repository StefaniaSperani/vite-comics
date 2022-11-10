<template>
    <section>
        <div class="container">
            <div>
            </div>

            <div>
            </div>
        </div>
    </section>

</template>

<script>
export default {
    name: 'Footer2Comp'
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as *;
@use '../assets/styles/partials/variables' as *;

section {
    background-color: $footer2;
    min-height: 7rem;

    .container {
        padding: 2em;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }



}
</style>