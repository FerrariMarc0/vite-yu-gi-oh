<script> 
    export default {
        name: 'Dropdown'
    }
</script>

<template>
    <div class="container-sm my-4">
        <form>
            <label for="search-type" class="d-none"></label>
            <select class="form-select-sm" id="search-type">
                <option selected>- Select -</option>
                <option value="1">Alien</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
            </select>
        </form>
    </div>
    
</template>

<style lang="scss" scoped>
    #search-type{
        width: 100px;
    }
</style>