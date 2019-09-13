<template>

        <v-img
                src="/images/Main/pic1.jpg"
                lazy-src="/images/Main/pic1.jpg"
                aspect-ratio="1"
                class="grey lighten-2"
                max-width="100%"
                max-height="500px"

        >
        <div id="col">
                <div class=" text-center">


                        <p class="display-1" >Reimagine home
                       </p>
                <p class="display-4" > We’ll help you find a place you’ll love.</p>
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
                    </v-col>
                    </div>
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