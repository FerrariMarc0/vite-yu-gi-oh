<script> 
import {store} from '../store'
    export default {
        name: 'Dropdown',
        data(){
            return {
                store
            }
            
        }
    }
</script>

<template>
    <div class="container-sm my-4">
        <form @change="$emit('search')">
            <label for="search-type" class="d-none"></label>
            <select class="form-select-sm" id="search-type" v-model="store.searchStatus">
                <option>- Select -</option>
                <option>Alien</option>
                <option>Abyss Actor</option>
                <option>Abyss Script</option>
                <option>Blaze Accelerator</option>
                <option>Cloudian</option>
                <option>Destiny HERO</option>
                <option>Empowered Warrior</option>
                <option>Fire King</option>
                <option>Gate Guardian</option>
                <option>Heroic</option>
                <option>Jinzo</option>
                <option>Knightmare</option>
                <option>Lady of Lament</option>
                <option>Magician</option>
            </select>
        </form>
    </div>
    
</template>

<style lang="scss" scoped>
    #search-type{
        width: 150px;
    }
</style>