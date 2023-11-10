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
.footer-social {
        background-color: var(--color-bg-footer);
        button {
            color: var(--color-light);
            border: 2px solid var(--color-primary);
            border-radius: 0;
        }
    }

</style>