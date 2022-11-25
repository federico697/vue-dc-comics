<template>
    <div class="fumetto">
        <img :src="datiFumetto.thumb" alt="">
        <h5>{{datiFumetto.series}}</h5>
    </div>
</template>

<script>
    export default {
        props: {
            datiFumetto: Object
        }
    }
</script>

<style lang="scss" scoped>

</style>