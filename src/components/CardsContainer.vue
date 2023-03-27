<script>
import {store} from '../store'
import CardsList from './CardsList.vue';
    export default {
        name: 'Cards container',
        components: {
            CardsList
        },
        data(){
            return {
                store,
                characters: []
            }
        }
        
    }
</script>

<template>
    <div class="bg-light m-auto" id="container">
        <div class="row g-3" v-for="character in store.characters">
            <div class="col-8  col-sm-2" >
                <CardsList id="card" :title="character.name" :species="character.archetype"/>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped> 
    #container{
        width: 1685px;
        height: 100vh;
    }
    #card{
        height: 200px;
        width: 150px;
        border: 1px solid;
    }
</style>