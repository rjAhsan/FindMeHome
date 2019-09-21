<template>
    <v-row justify="center">
        <v-dialog v-model="dialog" persistent max-width="600px">
            <template v-slot:activator="{ on }">
                <v-btn x-large  v-on="on">
                    <v-icon left>mdi-human-child</v-icon>
                    <span>SignUp</span>
                </v-btn>
            </template>
            <v-card>
                <v-card-title>
                    <div class="headline"><span class="text-center">Login</span></div>
                </v-card-title>
                <v-card-text>
                    <v-container>
                        <v-row>

                            <v-col cols="12" sm="6" m="4">
                                <v-text-field label="First-Name*"  required prepend-icon="mdi-email" v-model="name"></v-text-field>
                            </v-col>

                            <v-col cols="12" sm="6" m="4">
                                <v-text-field label="Last-Name*" required prepend-icon="mdi-email" v-model="name"></v-text-field>
                            </v-col>


                            <v-col cols="12">
                                <v-text-field label="PhoneNumber*" type="number" required prepend-icon="mdi-email" v-model="PhoneNumber"></v-text-field>
                            </v-col>





                            <v-col cols="12">
                                <v-text-field label="Email*" required prepend-icon="mdi-email" v-model="email"></v-text-field>
                            </v-col>

                            <v-col cols="12">
                                <v-text-field label="Password*" type="password" required prepend-icon="mdi-key" v-model="password"></v-text-field>
                            </v-col>

                            <v-col cols="12">
                                <v-text-field label="Conform-Password*" type="password" required prepend-icon="mdi-key" v-model="password"></v-text-field>
                            </v-col>


                        </v-row>
                    </v-container>
                    <small>*indicates required field</small>
                </v-card-text>
                <v-card-actions>
                    <div class="flex-grow-1"></div>
                    <v-btn class="error" dark @click="dialog = false">Close</v-btn>
                    <v-btn class="primary" dark @click="dialog = false">Login</v-btn>
                </v-card-actions>
            </v-card>
        </v-dialog>
    </v-row>
</template>
<script>
    export default {
        data: () => ({
            dialog: false,
            email:'',
            password:'',
        })
    }
</script>

<style scoped>

</style>