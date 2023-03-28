<script>
    export default {
        name: 'Header'
    }
</script>

<template>
    <header class="container-fluid d-flex px-5 py-2 gap-5 bg-light align-items-center">
        <div class="logo">
            <img src="../../public/img/logo.png" alt="img-logo">
        </div>
        <h1 class="text-center">Yu-Gi-Oh Api</h1>
    </header>
</template>

<style lang="scss" scoped>
    .logo{
        width: 6.25rem;
    }
</style>