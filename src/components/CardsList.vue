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
            <h5 class="text-white">{{title}}</h5>
        <span>{{ species }}</span> 
        </div>
        
    </article>
</template>