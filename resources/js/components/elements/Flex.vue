<template>
<div>
        <v-img
                src="/images/Main/pic1.jpg"
                lazy-src="/images/Main/pic1.jpg"
                aspect-ratio="1"
                class="grey lighten-2"
                max-width="100%"
                max-height="5%"
                min-height="1%"
        >
            <div class=" display-1 purple darken-2 text-center">
                <span class="white--text">Lorem ipsum</span>
            </div>
                <div class="text-center">
                    <h1 class="display-1" ><span class="white--text">Reimagine home.</span></h1>
                        <h1 class="display-3" > We’ll help you find a place you’ll love.</h1>
                    <br>
                    <br>



                    <div class="flex-grow-1">

                    <v-col cols="12" sm="12">
                        <v-text-field
                                label="Filled"
                                placeholder="Placeholder"
                                filled
                                append-outer-icon="mdi-help"
                        ></v-text-field>
                        <v-btn color="red" flat large >
                            <span class="white--text"> Search</span>

                        </v-btn>
                    </v-col>
                    </div>
                </div>




        </v-img>
    <div class="primary display-1 text-center">
        <span class="white--text">Lorem ipsum</span>
    </div>

        <!--<img src="/images/Main/pic1.jpg" alt="avatar">-->

</div>
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