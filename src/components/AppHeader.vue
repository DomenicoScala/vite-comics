<script>
    export default{
        data(){
            return{
                link: [
                    'CHARACTERS',
                    'COMICS',
                    'MOVIES',
                    'TV',
                    'GAMES',
                    'COLLECTIBLES',
                    'VIDEOS',
                    'FANS',
                    'NEWS',
                    'SHOP'
                ]

            };
        },
        methods:{

        }
    }
</script>

<template>

    <header>
            <div class="container">
                <div class="flex-header">
                    <div class="logo">
                        <img src="/img/dc-logo.png" alt="logo">
                    </div>

                    <div class="nav">
                        <nav>
                            <ul>
                                <li v-for="(link,i) in link">
                                    <a href="#">{{ link }}</a>
                                </li>
                            </ul>
                        </nav>
                    </div>
                </div>
            </div>
    </header>

</template>

<style lang="scss" scoped>
   @use "../assets/scss/main.scss" as *;
   
    header{
        height: 100px;
        margin-bottom: 20px;
    }


    img{
        width: 75%;
    }

    .flex-header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px;
    }

    li{
        display: inline-block;
        margin-right: 25px;
        
        > a{
            color: rgb(71, 71, 71);
            font-weight: bold;
        }
    }
</style>
