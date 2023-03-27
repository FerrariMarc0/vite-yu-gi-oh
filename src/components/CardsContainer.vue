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
    <div class="bg-light m-auto p-5" id="container">
        <div class="row p-2 mx-1 bg-black text-white">
            <span>Found 39 Cards</span>
        </div>
        <div class="row bg-light">
                <div class="col-12 col-sm-2 g-3" v-for="character in store.characters.data.slice(0,100)">
                    <CardsList class="px-1" id="card" :img="character.card_images[0].image_url" :title="character.name" :species="character.archetype"/>
                </div>
            </div>
        <div>
            
        </div>
    </div>
</template>

<style lang="scss" scoped> 
    #container{
        width: 1500px;
    }
    
</style>