<template>
    <v-container class="my-3">
        <v-card
                class="mx-2 px-2"
                max-width="100%"
                min-hight="80%"

        >
            <v-card-text>
                <div class="display-2 text-center  font-weight-bold ">
                    Popular Locations
                </div>
            </v-card-text>
            <v-layout row wrap class="ma-3 pa-3">
                <v-flex xm12 md4>
                    <v-card
                            class="mx-2 px-2"
                            max-width="100%"
                            min-hight="80%"

                    >
                        <v-card-text>
                            <div class="display-1 font-weight-bold text-left">
                                Most Popular Locations for Sale in Lahore
                            </div>
                            <hr>
                        </v-card-text>



                        <v-card-text v-for="(Lhr,i) in Lahores"
                        :key="i"
                        >
                        <v-btn
                        text
                        to=""
                        >
                            <h5>{{Lhr}}
                            </h5>
                        </v-btn>

                        </v-card-text>



                    </v-card>
                </v-flex>
                <v-flex xm12 md4>
                    <v-card
                            class="mx-2 px-2"
                            max-width="100%"
                            min-hight="80%"

                    >
                        <v-card-text>
                            <div class="display-1 font-weight-bold text-left">
                                Most Popular Locations for Sale in Lahore
                            </div>
                        </v-card-text>


                        <v-card-text v-for="(isb,i) in Islamabads"
                                     :key="i"
                        >
                            <v-btn
                                    text
                                    to=""
                            ><h5>
                                {{isb}}
                            </h5>
                            </v-btn>

                        </v-card-text>



                    </v-card>
                </v-flex>
                <v-flex xm12 md4>
                    <v-card
                            class="mx-2 px-2"
                            max-width="100%"
                            min-hight="80%"

                    >
                        <v-card-text>
                            <div class="display-1 font-weight-bold text-left">
                                Most Popular Locations for Sale in Karchi
                            </div>
                        </v-card-text>

                        <v-card-text v-for="(Kar,i) in Karchis"
                        :key="i">
                            <v-btn
                                    text
                                    to=""
                            ><h5>
                                {{Kar}}
                            </h5>
                            </v-btn>

                        </v-card-text>


                    </v-card>
                </v-flex>

            </v-layout>



        </v-card>
    </v-container>
</template>

<script>
    export default {
        data(){
            return{
                Lahores:[
                    'DHA',
                    'Bhari Town',
                    'Bahri Orchad',
                    'Lake city',
                    'StateLife Hosuing Socity',
                    'LDA AVENU',
                    'DHA RAHBER',
                    'Paragon city',
                    'Riwand Road',
                    'Gulberg',
                ],
                Islamabads:[
                    'DHA Defence',
                    'Gulberg',
                    'B-17',
                    'Bahria Town',
                    'D-12',
                    'G-14',
                    'I-12',
                    'I-14',
                    'F-17',
                    'G-13',

                ],
                Karchis:[
                    'Bahria Town Karachi',
                    'DHA Defence',
                    'Scheme 33',
                    'DHA City Karachi',
                    'Gadap Town',
                    'Bin Qasim Town',
                    'Scheme 45 ',
                    'Gulistan-e-Jauhar',
                    'Naya Nazimaba',
                    'Gulshan-e-Mehmood',

                ]


            }
        }
    }
</script>

<style scoped>

</style>