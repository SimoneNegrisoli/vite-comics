<template>
    <div>
        <img :src="imgCh" :alt="titleCh">
    </div>
    <div>
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