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
                ]

                

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
                            <li v-for="(icon,i) in iconsFooterUp">
                                <img :src="icon.icon" alt="">
                                <a href="#">{{ icon.name }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </section>

            <section>
                <div class="container">
                    
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
        background-image: url(../../public/img/footer-bg.jpg);
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
            text-decoration: none;
            color: white;
            cursor: pointer;
            vertical-align: middle;
            margin-left: 15px;
        }

    }

</style>
