<template>
<div>

         <nav-bar  ></nav-bar>
         <flex-image ></flex-image>

</div>
</template>

<script>

    import NavBar from '../elements/NavBarComponent.vue';
    import Flex from '../elements/Flex.vue';
    export default {

        components:{

            'nav-bar':NavBar,
            'flex-image':Flex,
        }
    }
</script>

<style scoped>
.img{
    overflow:visible;
}

</style>