<script>
import CardsContainer from './CardsContainer.vue';
import DropdownCharacter from './DropdownCharacter.vue';

    export default {
        name: 'Main',
        components: {
            DropdownCharacter,
            CardsContainer
        }
    }
</script>

<template>
    <DropdownCharacter/>
    <CardsContainer/>
</template>
                AppDropdown