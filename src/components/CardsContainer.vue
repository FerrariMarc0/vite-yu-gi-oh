<script>
import CardsList from './CardsList.vue';
    export default {
        name: 'Cards container',
        components: {
            CardsList
        }
    }
</script>

<template>
    <div class="bg-light m-auto" id="container">
        <div class="row">
            <div class="col-12 col-sm-4">
                <CardsList/>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #container{
        width: 1685px;
        height: 100vh;
    }
</style>