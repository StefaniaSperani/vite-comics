<template>
    <footer>
        <div class="container">
            <div class="list">
                <ul>
                    <span class="title">Dc Comics</span>
                    <li v-for="(comic, index) in comics" :key="index">
                        <a :href="comic.url">{{ comic.text }}</a>
                    </li>
                    <ul>
                        <span class="title">Shop</span>
                        <li v-for="(item, index) in shop" :key="index">
                            <a :href="item.url">{{ item.text }}</a>
                        </li>
                    </ul>
                </ul>
                <ul>
                    <span class="title">DC</span>
                    <li v-for="(term, index) in dc" :key="index">
                        <a :href="term.url">{{ term.text }}</a>
                    </li>
                </ul>
                <ul>
                    <span class="title">Sites</span>
                    <li v-for="(site, index) in sites" :key="index">
                        <a :href="site.url">{{ site.text }}</a>
                    </li>
                </ul>
            </div>

            <div class="imageFooter">
                <!-- IMG BACKGROUND -->
            </div>
        </div>

    </footer>
</template>

<script>
export default {
    name: 'FooterComp',
    data() {
        return {
            comics: [
                { text: "Characters", url: "#" },
                { text: "Comics", url: "#" },
                { text: "Movies", url: "#" },
                { text: "TV", url: "#" },
                { text: "Games", url: "#" },
                { text: "Videos", url: "#" },
                { text: "News", url: "#" },
            ],
            shop: [
                { text: "Shop DC", url: "#" },
                { text: "Shop DC Collectibles", url: "#" },
            ],
            dc: [
                { text: "Terms Of Use", url: "#" },
                { text: "Privacy policy (New)", url: "#" },
                { text: "Ad Choices", url: "#" },
                { text: "Advertising", url: "#" },
                { text: "Jobs", url: "#" },
                { text: "Subscriptions", url: "#" },
                { text: "Talent Workshops", url: "#" },
                { text: "CPSC Certificates", url: "#" },
                { text: "Ratings", url: "#" },
                { text: "Shop Help", url: "#" },
                { text: "Contact Us", url: "#" },
            ],
            sites: [
                { text: "DC", url: "#" },
                { text: "MAD Magazine", url: "#" },
                { text: "DC Kids", url: "#" },
                { text: "DC Universe", url: "#" },
                { text: "DC Power Visa", url: "#" },
            ],
        }
    },
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins' as *;
@use '../assets/styles/partials/variables' as *;

footer {
    background-image: url(../assets/img/footer-bg.jpg);
    min-height: 25rem;
    background-repeat: no-repeat;
    background-size: cover;
}

div {
    display: flex;
    justify-content: space-between;

    .container {
        padding: 0;
    }

    .list {
        display: flex;
        height: 100%;
    }

    .title {
        font-size: 1.5em;
        line-height: 3em;
        font-weight: bold;
        text-transform: uppercase;
    }

    .list>ul {
        padding: 1.7em;
    }

    li {
        list-style: none;
        line-height: 1.5em;

        a {
            text-decoration: none;
            color: $icons;
        }
    }

}


.imageFooter {
    width: 600px;
    height: 420px;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
}
</style>