<template>
<nav class="navbar navbar-expand-lg">
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarScroll" aria-controls="navbarScroll" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>
    <div  class="collapse navbar-collapse" id="navbarScroll">
        <ul class="d-flex column-gap-4 navbar-nav me-auto my-2 my-lg-0 navbar-nav-scroll" style="--bs-scroll-height: 100px;">
            <li class="text-uppercase nav-item" v-for="link in navLinks">
                <a href="#" class="nav-link-active" @click.prevent>{{link}}</a>
            </li>
        </ul>
    </div>
</nav>
</template>

<script>
    export default {
        name: 'HeaderNav',
        data(){
            return {
                navLinks:[
                'characters',
                'comics',
                'movies',
                'tv',
                'games',
                'collectibles',
                'videos',
                'fans',
                'news',
                'shop'
                ],

            }
        }
        
    }
</script>

<style scoped lang="scss">
nav {
    // font-family: $title-font;
}
li {
    font-family: var(--font-title);
    transform: scale(0.9,1.1);
    font-weight: bold;
    a{
        color: var(--color-dark);
        &:hover{
            color: var(--color-primary);
        }
    }
}
</style>