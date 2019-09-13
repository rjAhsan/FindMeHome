<template>
    <div class="container">
        <div>
        <Nav-Bar></Nav-Bar>
        </div>
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div class="card">
                    <div class="card-header">Main Component</div>

                    <div class="card-body">
                        <div>
                            <h1>Main Components</h1>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>

<script>
    import NavBar from './elements/NavBarComponent.vue'
    export default {
        components: {
            'Nav-Bar': NavBar,

        },
        mounted() {
            console.log('Component Main.')
        }
    }
</script>

<style scoped>

</style>