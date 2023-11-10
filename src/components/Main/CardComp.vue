<template>
    <div class="card">
        <img :src="imgCh" class="card-img-top" :alt="titleCh">
        <h5 class="card-title">{{ titleCh }}</h5>
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

<style lang="scss" scoped></style>