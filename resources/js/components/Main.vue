<template>
<div>
        <nav-bar></nav-bar>
        <div class="mx-4">
                <router-view></router-view>

        </div>
        <slider-el></slider-el>
        <footer-el class="py-4"></footer-el>
</div>
</template>

<script>
    import Welcome from './pages/Welcome.vue'

    import NavBar from './elements/NavBarComponent.vue';
    import Flex from './elements/Flex.vue';
    import Slider from './elements/carousel';
    import footer from './elements/footer';
    import Grid from './elements/Grid';

    export default {
        components:{

            'nav-bar':NavBar,
            'flex-image':Flex,
            'slider-el':Slider,
            'footer-el':footer,
            'Grid-el':Grid,
        },
        mounted() {
            console.log('Component Main.')
        }
    }
</script>

<style scoped>

</style>