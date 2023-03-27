<script>
    export default {
        name: 'Cards',
        props: {
            img: String,
            title: String,
            species: String
        }
    }
</script>

<template>
    <article class="text-center">
        <!-- <div class="img"><img :src="img"></div> -->
        <h3>{{title}}</h3>
        <span>{{ species }}</span>
    </article>
</template>

<style lang="scss" scoped>
    
</style>