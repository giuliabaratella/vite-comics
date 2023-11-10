<template>
    <main>
        <div id="jumbo">
        </div>
        <div class="container py-5">
            <div class="label text-uppercase fw-bold">Current Series</div>
            <div class="d-flex flex-wrap justify-content-center align-items-stretch align-content-stretch column-gap-3">
                <div v-for="el in comicsArray">
                    <Card :img="el.thumb" :title="el.series"/>
                </div>
            </div>
            <div class="text-center">
                <button class="button btn text-uppercase fw-bold">Load More</button>
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
    position: relative;
    .container{
        position: relative;
        .label{
        padding: 10px 25px;
        background-color: var(--color-primary);
        position: absolute;
        top:-30px;
        left: 0;
        transform: scale(0.9,1.1);
        font-size: 1.4em;
    }
    }
    

    #jumbo{
        height: 400px;
        overflow: hidden;
        background-image: url("/img/jumbotron.jpg");
        background-size: cover;

    }
    .button {
        background-color: var(--color-primary);
        color: var(--color-light);
        padding: 10px 50px;
        border-radius: 0;
        transform: scale(0.9,1.1);
    }
}
   
</style>