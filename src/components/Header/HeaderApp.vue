

<template>
    <header>
        <div class="container">
            <div class="row align-items-center pt-4">
                <div class="col-12 col-md-4">
                    <img src="../../assets/immagini/dc-logo.png" alt="" />
                </div>
                <ul class="nav nav-underline col-12 col-md-8">
                    <li class="nav-item" v-for="(link, index) in menu">
                        <a class="nav-link" aria-current="page" :href="link.url" :class="{ active: link.current }">
                            {{ link.text.toUpperCase() }}
                        </a>
                    </li>
                </ul>
            </div>

        </div>

    </header>
</template>

<script>

export default {
    name: "HeaderApp",
    data() {
        return {
            menu: [
                {
                    text: "Character",
                    url: "#",
                    current: false,
                },
                {
                    text: "Comics",
                    url: "#",
                    current: false,
                },
                {
                    text: "Movie",
                    url: "#",
                    current: false,
                },
                {
                    text: "Tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "Games",
                    url: "#",
                    current: true,
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "News",
                    url: "#",
                    current: false,
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false,
                },
            ],
        };
    },
};
</script>

<style lang="scss" scoped>
header {
    background-color: white;
    font-family: sans-serif;
}

div img {
    padding: 10px;
}
</style>
