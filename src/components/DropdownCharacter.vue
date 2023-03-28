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
                <option selected value="">- Select -</option>
                <option>Alien</option>
                <option>Noble Knight</option>
                <option>Melodius</option>
            </select>
        </form>
    </div>
    
</template>

<style lang="scss" scoped>
    #search-type{
        width: 150px;
    }
</style>