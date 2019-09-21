<template>
<nav class="img">

    <v-toolbar dense app extended >

        <v-btn light text x-large to="/Sale">Sale</v-btn>
        <v-btn light text x-large to="/Rent">Rent</v-btn>
        <v-btn light text x-large to="/Buy">Buy</v-btn>
        <v-btn light text x-large to="/Agentfinder">Agenet-Finder</v-btn>



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
        <logo-el>

        </logo-el>

        <v-spacer></v-spacer>

        <div class="flex-grow-1">

            </div>





        <v-btnt x-large>
                <login-el></login-el>
        </v-btnt>

        <v-btn x-large>
        <Signup-el ></Signup-el>
        </v-btn >

            <v-btn  x-large>
                <v-icon left>mdi-help</v-icon>
                <span>help</span>
            </v-btn>


        </v-toolbar>



</nav>

</template>

<script>
    import Logo from './Logo.vue';
    import Flex from './Flex.vue';
    import Login from './Login.vue';
    import Signup from './Signup.vue';
    export default {

        components:{
            'logo-el':Logo,
            'Fle-img':Flex,
            'login-el':Login,
            'Signup-el':Signup,

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
            },
            login(){
                console.log("Im Iron Man")
            }
        }
    }
</script>
<style scoped>
    .img{
        z-index: 5000;
        position: relative;

    }
    .nb{
        position: fixed;
    }
</style>