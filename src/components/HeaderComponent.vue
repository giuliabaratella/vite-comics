<template>
    <header>
        <div class="container d-flex justify-content-between align-items-center ">
            <div id="logo" class="my-3">
                <img src="/public/img/dc-logo.png" alt="DC Comics">
            </div>
            <HeaderNav/>
        </div>
    </header>
</template>

<script>

    import HeaderNav from './HeaderNav.vue'
    export default {
        components:{
            HeaderNav,
        },
        name: 'HeaderComponent',
    }
</script>

<style scoped lang="scss">

</style>