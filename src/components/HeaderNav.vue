<template>
    <nav class="navbar navbar-expand-lg">
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarScroll" aria-controls="navbarScroll" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div  class="collapse navbar-collapse" id="navbarScroll">
            <ul class="d-flex column-gap-4">
                <li class="text-uppercase" v-for="link in navLinks">
                    <a href="#" @click.prevent>{{link}}</a>
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
    font-weight: bold;
    a{
        color: var(--color-dark);
        &:hover{
            color: var(--color-primary);
        }
    }
}
</style>