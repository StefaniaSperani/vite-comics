<template>
    <header class="container">
        <a href="#">
            <img src="../assets/img/dc-logo.png" alt="">
        </a>
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url" :class="{ 'active': link.current }">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'HeaderComp',
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true,
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false,
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false,
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as *;
@use '../assets/styles/partials/variables' as *;

header {
    height: 7rem;
    font-size: 400;
    @include dflex;


    img {
        max-width: 70%;
    }

    ul {
        list-style: none;
        display: flex;
        text-transform: uppercase;
        overflow: hidden;


        li a {
            margin: 1.3rem;
            display: inline-block;
            color: $black;
            text-decoration: none;
            font-weight: 600;
            padding: 2.7rem 0;


            &.active,
            &:hover {
                border-bottom: 5px solid $lightblue;
                transition: 0.3s;
            }
        }
    }

}
</style>