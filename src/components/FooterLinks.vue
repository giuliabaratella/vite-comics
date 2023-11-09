<template>
    <div class="footer-links">
        <div class="container d-flex justify-content-between">
            <div class="d-flex column-gap-4 pt-4">
                <div>
                    <ul>
                        <li><h4 class="text-uppercase">Dc Comics</h4></li>
                        <li v-for="el in DcComics"><a href="#" @click.prevent>{{el}}</a></li>
                    </ul>
                    <ul>
                        <li><h4 class="text-uppercase">Shop</h4></li>
                        <li v-for="el in Shop"><a href="#" @click.prevent>{{el}}</a></li>
                    </ul>
                </div>
                <ul>
                    <li><h4 class="text-uppercase">DC</h4></li>
                    <li v-for="el in Dc"><a href="#" @click.prevent>{{el}}</a></li>
                </ul>
                <ul>
                    <li><h4 class="text-uppercase">Sites</h4></li>
                    <li v-for="el in Sites"><a href="#" @click.prevent>{{el}}</a></li>
                </ul>
            </div>
            <img id="dc-logo-bg" src="/public/img/dc-logo-bg.png" alt="DC Logo">
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
.footer-links{
    background-image: url('/public/img/footer-bg.jpg');
    background-size: cover;
        #dc-logo-bg {
            display: block;
            height: 350px;
            width: 600px;
            object-fit: none;
        }
    color: var(--color-light);
        a{
            color: var(--color-icons);
            font-weight: 500;
            font-size: 0.8em;
            &:hover{
                    color: var(--color-light);
                }
        }
    }
</style>