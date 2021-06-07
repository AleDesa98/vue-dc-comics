<template>
    <header>
        <a href="/">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
        </a>
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url" :class="{ active: link.current }">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: "Header",
    data: function() {
        return {
            links: [
                {
                    text: "characters",
                    url: "#characters",
                    current: false
                },
                {
                    text: "comics",
                    url: "#comics",
                    current: true
                },
                {
                    text: "movies",
                    url: "#movies",
                    current: false
                },
                {
                    text: "tv",
                    url: "#tv",
                    current: false
                },
                {
                    text: "games",
                    url: "#games",
                    current: false
                },
                {
                    text: "collectibles",
                    url: "#collectibles",
                    current: false
                },
                {
                    text: "videos",
                    url: "#videos",
                    current: false
                },
                {
                    text: "fans",
                    url: "#fans",
                    current: false
                },
                {
                    text: "news",
                    url: "#news",
                    current: false
                },
                {
                    text: "shop",
                    url: "#shop",
                    current: false
                }
            ]
        }
    }, 
    methods: {
        saluta: function() {
            alert("Ciao");
        }
    }
}
</script>

<style lang="scss" scoped>
    header {
        display: flex;
        justify-content: space-between;
        height: 120px;
        align-items: center;
    }

    header > a {
        margin: 10px;
    }

    .active {
        color: blue;
        border-bottom: 2px solid blue;
    }

    ul {
        display: flex;
        justify-content: center;
        align-items: center;
        list-style: none;

        li {
            a {
                padding: 10px;
                color: black;
                text-decoration: none;
                text-transform: uppercase;
            }
        }
    }
</style>