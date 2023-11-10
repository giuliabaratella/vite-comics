<template>
    <div class="d-flex column-gap-3 align-items-center">
        <div class="text-uppercase fw-bold follow-us d-none d-md-block">Follow us</div>
        <div class="d-flex column-gap-3 align-items-center ">
            <a href="#" @click.prevent v-for="el in socialIcons">
                <img :src=el alt="social media link">
            </a>
        </div>
    </div>
</template>

<script>
    export default {
        name:'SocialIcons',
        data(){
            return{
                socialIcons:[
                    '/img/footer-fb.png',
                    '/img/footer-twit.png',
                    '/img/footer-youtube.png',
                    '/img/footer-pinterest.png',
                    '/img/footer-periscope.png',
                    ]
                }

            }
    }
</script>

<style scoped lang="scss">
.follow-us{
            color: var(--color-primary);
            font-size: 1.1em;
            transform: scale(1,1.5);

            
        }
    a img:hover{
            opacity: 80%;
        }
</style>