<template>
    <div class="my-2">
        <div class="mycard-c">
            <img :src="imgCh" :alt="titleCh">
        </div>
        <div class="my-2">
            <h6 class="card-title">{{ titleCh }}</h6>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardComp',
    props: {
        imgCh: String,
        titleCh: String
    }
}
</script>

<style lang="scss" scoped>
.mycard-c {
    width: 100%;
    height: 180px;
    overflow: hidden;

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
    }
}
</style>