<template>
    <section>
        <div class="container">
            <div>
                <a href="#">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital">
                    <span>Digital Comics</span>
                </a>
            </div>
            <div>
                <a href="#">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="Merch">
                    <span>Dc Merchandise</span>
                </a>
            </div>
            <div>
                <a href="#">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="Subs">
                    <span>Subscription</span>
                </a>
            </div>
            <div>
                <a href="#">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="Shops">
                    <span>Comic Shop Locator</span>
                </a>
            </div>
            <div>
                <a href="#">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="Visa">
                    <span>Dc Power Visa</span>
                </a>
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
    padding: 2em;
    @include merchStyle;


    a {
        padding: 1.5rem;
        text-decoration: none;
        @include merchStyle;
    }
}

img {
    width: 50%;
}

span {
    padding: 0 1.5rem;
}
</style>