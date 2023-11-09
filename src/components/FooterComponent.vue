<template>
<footer>
    <FooterLinks/>
    <FooterSocial/>
</footer>
</template>

<script>
import FooterLinks from './FooterLinks.vue'
import FooterSocial from './FooterSocial.vue'

    export default {
        name: 'FooterComponent',
        components:{
            FooterLinks,
            FooterSocial,
        },
    }
</script>

<style scoped>
</style>