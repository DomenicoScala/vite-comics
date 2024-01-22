<script>
    export default{
        data(){
            return{
                iconsFooterUp : [
                    {
                        name: 'DIGITAL COMICS',
                        icon: '/img/buy-comics-digital-comics.png'
                    },
                    {
                        name:'DC MERCHANDISE',
                        icon: '/img/buy-comics-merchandise.png'
                    },
                    {
                        name: 'SUBSCRIPTION',
                        icon: '/img/buy-comics-subscriptions.png'
                    },
                    {
                        name: 'COMIC SHOP LOCATOR',
                        icon: '/img/buy-comics-shop-locator.png'
                    }
                ],

                
                

            };
        },
        methods:{

        }
    }
</script>

<template>

        <footer>
            <section>
                <div class="container">
                    <div class="footer-up">
                        <ul>
                            <li v-for="(icon,i) in iconsFooterUp" :key="i">
                                <img :src="icon.icon" alt="">
                                <a href="#">{{ icon.name }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </section>

            <section>
                <div class="container">
                    <div class="footer-bottom">
                        <div>
                            <h4>
                                DC COMICS
                            </h4>

                            <ul>
                                <li>
                                    <a href="#">
                                       Characters
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Comics
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Movies
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        TV
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                       Games
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                       Videos
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                       News
                                    </a>
                                </li>
                            </ul>

                            <h4>
                                SHOP
                            </h4>

                            <ul>
                                <li>
                                    <a href="#">
                                       Shop DC
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Shop DC Collectibles
                                    </a>
                                </li>
                            </ul>
                        </div>

                        <div>
                            <h4>
                                DC
                            </h4>

                            <ul>
                                <li>
                                    <a href="#">
                                       Terms Of Use
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Privacy policy(New)
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Ad Choices
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Advertising
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                       Jobs
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                       Subscription
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                       Talent Workshops
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                       CPSC Certificates
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                       Ratings
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                       Shop Help
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                       Contact Us
                                    </a>
                                </li>
                            </ul>
                        </div>

                        <div>
                            <h4>
                                SITES
                            </h4>

                            <ul>
                                <li>
                                    <a href="#">
                                       DC
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Mad Magazine
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        DC Kids
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        DC Universe
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                       DC Power Visa
                                    </a>
                                </li>
                            </ul>
                        </div>

                        <!-- <div>
                            <img src="/img/dc-logo-bg.png" alt="">
                        </div> -->
                    </div>
                </div>
            </section>

            <section>
                <div class="container">
                    <div class="flex-footer-bottom2">
                        <div>
                            <a href="#"> SIGN-UP NOW</a>
                        </div>

                        <div>
                            <h4>FOLLOW US</h4>
                            <ul>
                                <li>
                                    <img src="/img/footer-facebook.png" alt="">
                                </li>
                                <li>
                                    <img src="/img/footer-twitter.png" alt="">
                                </li>
                                <li>
                                    <img src="/img/footer-youtube.png" alt="">
                                </li>
                                <li>
                                    <img src="/img/footer-periscope.png" alt="">
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </section>
        </footer>

</template>

<style lang="scss" scoped>
    @use "../assets/scss/main.scss" as *;

    footer section:nth-child(1){
        background-color: #0282F9;
    }

    footer section:nth-child(2){
        background-image: url(/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }

    footer section:nth-child(3){
        background-color:#303030;
    }

    .footer-up{
        padding: 20px;
    }

    li{
        display: inline-block;
        margin: 25px;
        text-align: center;

        > img{
            max-width: 20%;
            cursor: pointer;
            vertical-align: middle;
            
        }

        &:last-child{
             > img{
               max-width: 15%;
             }

        }

        > a{
            color: white;
            cursor: pointer;
            vertical-align: middle;
            margin-left: 15px;
        }

    }

    .footer-bottom{
        display: flex;
        padding: 50px;

        > div h4{
            color: white;
            margin: 10px 20px;
            font-size: 20px;
            font-weight: bold;
                        
        }

        > div img{
            width: 70%;
        }

        
    }

    .footer-bottom ul li{
        display: block;
        margin: 3px;
        text-align: start;
        
        & a{
            color: gray;
            font-size: 12px;
        }

    }

    .flex-footer-bottom2{
        display: flex;
        justify-content: space-between;
        padding: 10px;
    }


</style>
