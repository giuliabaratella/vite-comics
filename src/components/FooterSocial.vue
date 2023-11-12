<template>
    <div class="footer-social">
        <div class="container d-flex justify-content-between py-5">
            <button class="btn text-uppercase fw-bold">Sign-up now!</button>
            <SocialIcons/>
        </div>
    </div>
</template>

<script>
import SocialIcons from './SocialIcons.vue'
    export default {
        name:'FooterSocial',
        components:{
            SocialIcons,
        }

    }
</script>

<style scoped lang="scss">
@use '../assets/styles/partials/variables.scss' as *;

.footer-social {
        background-color: $color-bg-footer;
        button {
            color: $color-light;
            border: 2px solid $color-primary;
            border-radius: 0;
        }
    }

</style>