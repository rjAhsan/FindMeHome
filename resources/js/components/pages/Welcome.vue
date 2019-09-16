<template>
<div>

         <nav-bar  ></nav-bar>
        <div class="mx-4">
         <flex-image ></flex-image>
         <Grid-el></Grid-el>
         <slider-el></slider-el>
         <footer-el class="py-4"></footer-el>
        </div>
</div>
</template>

<script>

    import NavBar from '../elements/NavBarComponent.vue';
    import Flex from '../elements/Flex.vue';
    import Slider from '../elements/carousel';
    import footer from '../elements/footer';
    import Grid from '../elements/Grid';
    export default {

        components:{

            'nav-bar':NavBar,
            'flex-image':Flex,
            'slider-el':Slider,
            'footer-el':footer,
            'Grid-el':Grid,
        }
    }
</script>

<style scoped>
.img{
    overflow:visible;
}

</style>