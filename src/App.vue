<script>
    import AppHeader from './components/AppHeader.vue'
    import AppMain from './components/AppMain.vue'
    import AppFooter from './components/AppFooter.vue'
    
    export default{
        data(){
            return{

            };
        },
        methods:{

        },
        components:{
            AppHeader,
            AppMain,
            AppFooter
        }
    }
</script>

<template>

        <h1>
            Mia App
        </h1>

        <AppHeader/>

        <AppMain/>

        <AppFooter/>

</template>

<style lang="scss">
    @use "assets/scss/main.scss" as *;
    @import "assets/scss/partials/reset.scss";
</style>
