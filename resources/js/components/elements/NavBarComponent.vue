<template>
<nav class="img">
        <v-toolbar dense>

            <logo-el></logo-el>
            <v-spacer></v-spacer>
            <div class="text-center">
                <v-menu open-on-hover dark top >
                    <template v-slot:activator="{ on }">
                        <v-btn

                                dark
                                v-on="on"
                        >
                            Rent
                        </v-btn>
                    </template>

                    <v-list>
                        <v-list-item
                                v-for="(item, index) in items"
                                :key="index"
                                @click=""
                        >
                            <v-list-item-title>{{ item.title }}</v-list-item-title>
                        </v-list-item>
                    </v-list>
                </v-menu>
            </div>

            <div class="text-center">
                <v-menu open-on-hover dark top >
                    <template v-slot:activator="{ on }">
                        <v-btn

                                dark
                                v-on="on"
                        >
                            Sell
                        </v-btn>
                    </template>

                    <v-list>
                        <v-list-item
                                v-for="(item, index) in items"
                                :key="index"
                                @click=""
                        >
                            <v-list-item-title>{{ item.title }}</v-list-item-title>
                        </v-list-item>
                    </v-list>
                </v-menu>
            </div>

                    <div class="text-center">
                        <v-menu open-on-hover dark top  >
                            <template v-slot:activator="{ on }">
                                <v-btn
                                        dark
                                        v-on="on"


                                >
                                    Buy
                                </v-btn>
                            </template>

                            <v-list>
                                <v-list-item
                                        v-for="(item, index) in items"
                                        :key="index"
                                        @click=""
                                >
                                    <v-list-item-title>{{ item.title }}</v-list-item-title>
                                </v-list-item>
                            </v-list>
                        </v-menu>
                    </div>

                    <div class="text-center">
                        <v-menu open-on-hover dark top >
                            <template v-slot:activator="{ on }">
                                <v-btn
                                        dark
                                        v-on="on"
                                >
                                    Agent-Finder
                                </v-btn>
                            </template>

                            <v-list>
                                <v-list-item
                                        v-for="(item, index) in items"
                                        :key="index"
                                        @click=""
                                >
                                    <v-list-item-title>{{ item.title }}</v-list-item-title>
                                </v-list-item>
                            </v-list>
                        </v-menu>
                    </div>







            <div class="flex-grow-1">

            </div>


                <v-btn text samll>Advertise</v-btn>
                <v-btn text samll>List your rentel</v-btn>



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



</nav>
</template>

<script>
    import Logo from './Logo.vue';
    import Flex from './Flex.vue';
    export default {
        components:{
            'logo-el':Logo,
            'Fle-img':Flex,

        },
        data: () => ({
            items: [
                { title: 'Click Me' },
                { title: 'Click Me' },
                { title: 'Click Me' },
                { title: 'Click Me 2' },
            ],
            offsetoverflow:true,
            offsety:true,
            zvalue:5000,

        }),
    }
</script>
<style scoped>
    .img{
        z-index: 5000;
        position: relative;
    }
</style>