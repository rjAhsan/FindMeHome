<template>

        <v-img
                src="c"
                lazy-src="/images/Main/pic1.jpg"
                aspect-ratio="1"
                class="grey lighten-2  "
                max-width="100%"
                max-height="700px"

        >

                <div class="text-center">
                    <h1 class="display-4 " ><span class="white--text">Reimagine home.</span></h1>
                    <h1 class="display-2 white--text" > We’ll help you find a place you’ll love.</h1>

                    <br>
                    <br>

                    <div class="flex-grow-1">

                    <v-col cols="8" sm="8" offset="sm-2">
                        <v-text-field class="text-bold text-uppercase"
                                dark
                                label="Search Home "
                                append-icon="mdi-magnify"
                                placeholder="Please Enter Location"
                                height="50px"
                        ></v-text-field>
                        <v-btn color="red"  large dark x-large  >
                            <v-icon left>mdi-magnify</v-icon>
                            <span class="white--text">Search</span>
                        </v-btn>
                    </v-col>
                    </div>
                </div>




        </v-img>


        <!--<img src="/images/Main/pic1.jpg" alt="avatar">-->


</template>

<script>
    export default {

    }
</script>

<style scoped>
    #col{
    color:white;

    }

</style>