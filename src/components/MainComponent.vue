<template>
    <main>
        <div></div>
        <div class="container py-5">
            <div class="d-flex flex-wrap justify-content-center align-items-stretch align-content-stretch column-gap-3">
                <div v-for="el in comicsArray">
                    <Card :img="el.thumb" :title="el.series"/>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
    import Card from './Card.vue'
    import {Comics} from '../data/dc-comics';
    export default {
        name: 'MainComponent',
        components:{
            Card
        },
        data(){
            return{
                comicsArray: Comics,
            }
        }
    }
</script>

<style scoped lang="scss">
main {
    color: var(--color-light);
    background-color: var(--color-dark);
}
   
</style>