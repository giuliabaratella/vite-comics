<template>
    <nav>
        <ul class="d-flex column-gap-4">
            <li class="text-uppercase" v-for="link in navLinks">
                <a href="#" @click.prevent>{{link}}</a>
            </li>
        </ul>
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
li {
    font-weight: bold;
    list-style-type: none;
    a{
        text-decoration: none;
    }
}
</style>