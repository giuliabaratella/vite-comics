<template>
    <div class="footer-social">
        <div class="container d-flex justify-content-between py-5">
            <button class="btn text-uppercase fw-bold">Sign-up now!</button>
            <div class="d-flex column-gap-3 align-items-center">
                <div class="text-uppercase fw-bold follow-us">Follow us</div>
                <a href="#" class="d-flex justify-content-center align-items-center" @click.prevent>F</a>
                <a href="#" class="d-flex justify-content-center align-items-center" @click.prevent>T</a>
                <a href="#" class="d-flex justify-content-center align-items-center" @click.prevent>Y</a>
                <a href="#" class="d-flex justify-content-center align-items-center" @click.prevent>P</a>
                <a href="#" class="d-flex justify-content-center align-items-center" @click.prevent>G</a>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:'FooterSocial',

    }
</script>

<style scoped lang="scss">
.footer-social {
        background-color: var(--color-bg-footer);
        button {
            color: var(--color-light);
            border: 2px solid var(--color-primary);
        }
        .follow-us{
            color: var(--color-primary);
            font-size: 1.5em;
        }
        a{
            width: 40px;
            height: 40px;
            padding: 10px;
            border-radius: 50%;
            background-color: var(--color-icons);
            color: var(--color-dark);
        }
    }

</style>