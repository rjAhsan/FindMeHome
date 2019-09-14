<template>

        <Wel-come></Wel-come>

</template>

<script>
    import Welcome from './pages/Welcome.vue'
    export default {
        components: {
            'Wel-come': Welcome,

        },
        mounted() {
            console.log('Component Main.')
        }
    }
</script>

<style scoped>

</style>