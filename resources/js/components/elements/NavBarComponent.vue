<template>
<nav class="img">

    <v-toolbar dense app extended>


            <div class="text-center">
                <v-menu open-on-hover light top >
                    <template v-slot:activator="{ on }">
                        <v-btn
                                large
                                light
                                v-on="on"
                                text
                        >
                            Rent
                        </v-btn>
                    </template>

                    <v-list>
                        <v-list-item
                                v-for="(item, index) in items"
                                :key="index"
                                @click="findname(item.title)"
                        >
                            <v-list-item-title>{{ item.title }}</v-list-item-title>
                        </v-list-item>
                    </v-list>
                </v-menu>
            </div>

            <div class="text-center">
                <v-menu open-on-hover light top >
                    <template v-slot:activator="{ on }">
                        <v-btn
large
text
                                light
                                v-on="on"
                        >
                            Sell
                        </v-btn>
                    </template>

                    <v-list>
                        <v-list-item
                                v-for="(item, index) in items"
                                :key="index"
                                @click="findname(item.title)"
                        >
                            <v-list-item-title>{{ item.title }}</v-list-item-title>
                        </v-list-item>
                    </v-list>
                </v-menu>
            </div>

                    <div class="text-center">
                        <v-menu open-on-hover light top  >
                            <template v-slot:activator="{ on }">
                                <v-btn
                                        large
                                        light
                                        v-on="on"
            text

                                >
                                    Buy
                                </v-btn>
                            </template>

                            <v-list>
                                <v-list-item
                                        v-for="(item, index) in items"
                                        :key="index"
                                        @click="findname(item.title)"
                                >
                                    <v-list-item-title>{{ item.title }}</v-list-item-title>
                                </v-list-item>
                            </v-list>
                        </v-menu>
                    </div>

        <div class="text-center">
            <v-menu open-on-hover light top  >
                <template v-slot:activator="{ on }">
                    <v-btn
                            light
                            v-on="on"
                            large
                            text


                    >
                        Agent-Finder
                    </v-btn>
                </template>

                <v-list>
                    <v-list-item
                            v-for="(item, index) in items"
                            :key="index"
                            @click="findname(item.title)"
                    >
                        <v-list-item-title>{{ item.title }}</v-list-item-title>
                    </v-list-item>
                </v-list>
            </v-menu>
        </div>
        <v-divider
                class="mx-1"
                vertical
        ></v-divider>
        <v-spacer></v-spacer>
        <logo-el></logo-el>





        <div class="flex-grow-1">

            </div>


                <v-btn text samll>Advertise</v-btn>
                <v-btn text samll>List your rentel</v-btn>



            <v-btn >
                <span>Login</span>
                <v-icon right>mdi-human-child</v-icon>

            </v-btn>

            <v-btn >
                <v-icon left>mdi-power</v-icon>
                <span>SingUp</span>
            </v-btn>

            <v-btn >
                <v-icon left>mdi-help</v-icon>
                <span>help</span>
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
        methods: {
            findname(refName) {
             console.log (refName);
            }
        }
    }
</script>
<style scoped>
    .img{
        z-index: 5000;
        position: relative;
    }
</style>