<script>
    export default{
        data(){
            return{

            };
        },
        methods:{

        },
        props:{
            fumetto: Object
        }
    }
</script>

<template>
    
    <div class="single-comic">
        <img :src="fumetto.thumb" alt="">
        <div>
            <h4>{{ fumetto.series }}</h4>
        </div>
    </div>

</template>

<style lang="scss" scoped>
    @use "../assets/scss/main.scss" as *;
    
    .single-comic{
        margin-bottom: 30px;
        
        > img{
            margin-bottom: 10px;
            width: 50%;
        }

        >div h4{
            color:white;
        }
    }
</style>
