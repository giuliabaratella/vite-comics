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
@use '../assets/styles/partials/variables.scss' as *;

main {

    color: $color-light;
    background-color: $color-dark;
    .container{
        position: relative;
        .label{
        padding: 8px 25px;
        background-color: $color-primary;
        position: absolute;
        top:-25px;
        left: 0;
        @include condensed;
        font-size: 1em;
    }
    }
    

    #jumbo{
        height: 400px;
        // overflow: hidden;
        background-image: url("/img/jumbotron.jpg");
        background-size: cover;

    }
    .button {
        background-color: $color-primary;
        color: $color-light;
        padding: 8px 50px;
        border-radius: 0;
        @include condensed;
        font-size:0.8em;
    }
}
   
</style>