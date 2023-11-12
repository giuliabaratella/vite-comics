<template>
    <div class="footer-links overflow-y-auto overflow-x-hidden">
        <div class="container d-flex justify-content-between h-100">
            <div class="pt-4 d-flex flex-column flex-wrap column-gap-4 h-100">
                <ul>
                    <li><h4 class="text-uppercase">Dc Comics</h4></li>
                    <li v-for="el in DcComics"><a href="#" @click.prevent>{{el}}</a></li>
                </ul>
                <ul>
                    <li><h4 class="text-uppercase">Shop</h4></li>
                    <li v-for="el in Shop"><a href="#" @click.prevent>{{el}}</a></li>
                </ul>
                <ul>
                    <li><h4 class="text-uppercase">DC</h4></li>
                    <li v-for="el in Dc"><a href="#" @click.prevent>{{el}}</a></li>
                </ul>
                <ul>
                    <li><h4 class="text-uppercase">Sites</h4></li>
                    <li v-for="el in Sites"><a href="#" @click.prevent>{{el}}</a></li>
                </ul>
            </div>
            <img id="dc-logo-bg" src="/img/dc-logo-bg.png" alt="DC Logo">
        </div>
    </div>
</template>

<script>
    export default {
        name:'FooterLinks',
        data(){
            return {
                DcComics:[
                    'Characters',
                    'Comics',
                    'Movies',
                    'TV',
                    'Games',
                    'Videos',
                    'News',
                ],
                Shop:[
                    'Shop DC',
                    'Shop DC Collectibles',
                ],
                Dc:[
                    'Term of use',
                    'Privacy policy(New)',
                    'Add Choices',
                    'Advertising',
                    'Jobs',
                    'Subscriptions',
                    'Talent Workshops',
                    'CPSC Certificates',
                    'Ratings',
                    'Shop Help',
                    'Contact Us',
                ],
                Sites:[
                    'DC',
                    'MAD Magazine',
                    'DC Kids',
                    'DC Universe',
                    'DC Power Visa',
                ],
            }
        }
    }
</script>

<style scoped lang="scss">
@use '../assets/styles/partials/variables.scss' as *;

.footer-links{
    background-image: url('/img/footer-bg.jpg');
    background-size: cover;
    height: 350px;
    color: $color-light;
    #dc-logo-bg {
        display: block;
        height: 350px;
        width: 600px;
        object-fit: none;
        overflow-x:visible;
        z-index:500;
    }
    h4{
        @include condensed;
        font-size: 1em;
    }
    a{
        color: $color-icons;
        font-weight: 500;
        font-size: 0.8em;
        z-index: 1000;
        &:hover{
                color: $color-light;
         }
    }
}
</style>