<script>
import CardsContainer from './CardsContainer.vue';
import DropdownCharacter from './DropdownCharacter.vue';

    export default {
        name: 'Main',
        components: {
            DropdownCharacter,
            CardsContainer
        },
        methods: {
            handleSearch(){
                this.$emit('find')
            }
        }
    }
</script>

<template>
    <DropdownCharacter @search="handleSearch"/>
    <CardsContainer/>
</template>