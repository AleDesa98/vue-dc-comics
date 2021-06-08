<template>
    <div class="card">
        <img :src="item.thumb" alt="">
        <div class="title"> {{item.series}} </div>
    </div>
</template>

<script>
export default {
    name: "Card",
    props: ["item"]
}
</script>

<style lang="scss" scoped>
    .card {
        width: calc(100% / 6);
        img {
            display: block;
        }
        .title {
            color: white;
            margin-top: 10px;
            text-transform: uppercase;
            font-size: 12px;
            margin-bottom: 50px;
        }
    }
</style>