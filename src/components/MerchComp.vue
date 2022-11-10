<template>
    <section>
        <div class="container">
            <div>
                <a href="#">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital">
                </a>
                <span>Digital Comics</span>
            </div>
            <div>
                <a href="#">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="Merch">
                </a>
                <span>Dc Merchandise</span>
            </div>
            <div>
                <a href="#">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="Subs">
                </a>
                <span>Subscription</span>
            </div>
            <div>
                <a href="#">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="Shops">
                </a>
                <span>Comic Shop Locator</span>
            </div>
            <div>
                <a href="#">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="Visa">
                </a>
                <span>Dc Power Visa</span>
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as *;
@use '../assets/styles/partials/variables' as *;

section {
    background-color: $lightblue;
    min-height: 250px;
}

div {
    padding: 2em 0.6em;
    @include merchStyle;


    a {
        text-decoration: none;
        @include merchStyle;
    }
}

img {
    width: 60px;
    height: 76px;
}

span {
    padding: 0 1.5rem;
    cursor: pointer;
    width: max-content;
}
</style>