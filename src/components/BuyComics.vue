<template>
    <div id="resources">
        <div class="container">
            <ul class="d-flex justify-content-evenly align-items-center row-gap-4 column-gap-4 m-0 py-5 flex-wrap">
                <li v-for="el in buyComics">
                    <a href="#" @click.prevent>
                        <div class="d-flex align-items-center">
                            <div class="pe-2" id="img-box">
                                <img :src=el.img :alt=el.text>
                            </div>
                            <div class="text-white text-uppercase">{{el.text}}</div>
                        </div>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'BuyComics',
        data(){
            return {
            buyComics:[
                {
                img:'/img/buy-comics-digital-comics.png',
                text:'Digital Comics'
                },
                {
                img:'/img/buy-comics-merchandise.png',
                text:'DC Merchandise'
                },
                {
                img:'/img/buy-comics-subscriptions.png',
                text:'Subscription'
                },
                {
                img:'/img/buy-comics-shop-locator.png',
                text:'Comic Shop Locator'
                },
                {
                img:'/img/buy-dc-power-visa.svg',
                text:'DC Power Visa'
                }
            ]
            }


        }
    }
</script>

<style scoped lang="scss">
#resources {
    background-color: var(--color-primary);
    #img-box {
        width: 50px;
        img {
            width: 100%;
        }
    }
    a:hover {
        background-color: var(--color-dark);
    }
}
</style>