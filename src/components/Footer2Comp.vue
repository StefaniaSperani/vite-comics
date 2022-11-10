<template>
    <section>
        <div class="container">
            <button><a href="#">Sign-Up Now!</a></button>

            <div class="follow-us">
                <h2>Follow us</h2>
                <img src="../assets/img/footer-facebook.png" alt="Facebook" />
                <img src="../assets/img/footer-twitter.png" alt="Twitter" />
                <img src="../assets/img/footer-youtube.png" alt="YouTube" />
                <img src="../assets/img/footer-pinterest.png" alt="Pinterest" />
                <img src="../assets/img/footer-periscope.png" alt="Periscope" />

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
    height: 7rem;

    .container {
        min-height: 100%;
        padding: 2em;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    button {
        background-color: transparent;
        border: 2px solid $lightblue;
        padding: 1rem;
        text-transform: uppercase;
        font-weight: bold;

        a {
            color: #fff;
            text-decoration: none;
        }
    }

    .follow-us {
        display: flex;
        gap: 17px;

        h2 {
            text-transform: uppercase;
            color: $lightblue;
            margin: 0 0.5em;
        }

        img {
            cursor: pointer;
        }
    }



}
</style>