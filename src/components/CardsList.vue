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
        <div class="img"><img :src="img"></div>
        <div class="art_bottom">
            <h6 class="text-white text-uppercase fw-bolder">{{title}}</h6>
            <span>{{ species }}</span> 
        </div>
        
    </article>
</template>