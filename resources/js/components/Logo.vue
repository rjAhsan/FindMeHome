<template>

    <v-card
            color="black lighten-4"
            dark
            height="10px"
            tile
    >
        <v-toolbar dense>

            <!--<v-app-bar-nav-icon></v-app-bar-nav-icon>-->
            <v-toolbar-title><i>Find<b>Me</b>House</i></v-toolbar-title>

            <div class="flex-grow-1">

            </div>

            <v-btn icon>
                <v-icon >mdi-human-child</v-icon>
            </v-btn>

            <v-btn icon>
                <v-icon>mdi-power</v-icon>
            </v-btn>

            <v-btn icon>
                <v-icon>mdi-help</v-icon>
            </v-btn>
        </v-toolbar>
    </v-card>


</template>

<script>
    export default {
        name: "Logo",
        data () {
            return {

            }
        },
    }
</script>

<style scoped>

</style>