<template>
    <v-footer
            light

    >
        <v-card
                flat
                tile
                class="grey darken-1  white--text text-center"
        >
            <v-layout row wrap class="ma-3 pa-3">
                <v-flex xm12 md4>

<div class="display-2 text-bold my-3">
    FindMeHouse.com
</div>

                    <div class="my-5">
                    <v-icon color="red" x-large>
                        mdi-map-marker
                    </v-icon >
                        <span class="display-1 text-center my-3">
                            Pearl One,
93-XYZ/I, YZ ABC Road,
Gulberg 43, Lahore,
Pakistan. </span>
                    </div >
                    <br>

                    <div class="my-5">
                        <v-icon color="blue" x-large>
                            mdi-phone
                        </v-icon >
                        <span class="display-1 text-center my-3">

+923067395766 </span>
                    </div >
<br>
                    <div class="my-5">
                        <v-icon color="green" x-large>
                            mdi-email
                        </v-icon >
                        <span class="display-1 text-center my-3">

info@findmehouse.com </span>
                    </div >
                    <br>







                    <v-btn
                                    v-for="icon in icons"
                                    :key="icon"
                                    class="mx-4 my-3  blue white--text"
                                    icon
                                    x-large
                                    fab
                            >
                                <v-icon >{{ icon }}</v-icon>
                            </v-btn>



<br>


                </v-flex>
                <v-flex xm12 md4>

                    <div class="display-2 text-bold my-3">
                        Company
                    </div>

<div v-for="link in links"
                    :key="link" >
                    <v-btn

                            color="white"
                          text
                            class="my-2"
                            x-large
                    >

                        <h4 class="text-uppercase  ">
                            {{ link }}
                        </h4>
                    </v-btn>
</div>



                </v-flex>
                <v-flex xm12 md4>

                    <div class="display-2 text-bold my-3">
                     Connect
                    </div>


                                <v-btn
                                        v-for="link in linkss"
                                        :key="link"
                                        color="white"
                                        text
                                        rounded
                                        class="my-2"
                                        x-large
                                >

    <h4 class="text-uppercase ">
                                    {{ link }}
    </h4>
                                </v-btn>




                </v-flex>
                <v-col
                        class=" blue my-3 py-4 text-center white--text"
                        cols="12"
                        dark
                >
                    <strong><h3>Copyright 2009 - 2022 FindMeHouse.com
                    All Rights Are Reserved.
                    Official Home Partners
                    </h3></strong>
                </v-col>
            </v-layout>


        </v-card>

    </v-footer>
</template>

<script>
    export default {
        data: () => ({
            icons: [
                'mdi-facebook',
                'mdi-twitter',
                'mdi-google-plus',
                'mdi-instagram',
            ],
            linkss: [
                'News',
                'Blogs',
                'Forum',
                'Expo',
                'Add Property',

            ],


            links: [
                'Home',
                'About Us',
                'Team',
                'Services',
                'Blog',
                'Contact Us',
            ],
        }),
    }
</script>

<style scoped>

</style>