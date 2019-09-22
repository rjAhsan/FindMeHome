<template>

   <v-card
           class="mx-2 px-2 py-4"
           max-width="100%"
           min-hight="80%"
   >
   <vv-card-text
       <div class="text-center display-3 text-bold">Titanium Agencies</div>
   </v-card-text>
       <v-carousel
            cycle
            height="250"
            hide-delimiter-background
            show-arrows-on-hover
            class="py-3"
    >
        <v-carousel-item
                v-for="(slide, i) in slides"
                :key="i"
        >
            <v-sheet
                    :color="colors[i]"
                    height="100%"
            >
                <v-row
                        class="fill-height"
                        align="center"
                        justify="center"
                >
                    <div class="display-3">{{ slide }} Slide</div>
                </v-row>
            </v-sheet>
        </v-carousel-item>
    </v-carousel>
   </v-card>

</template>

<script>
    export default {
        data() {
            return {
                colors: [
                    'indigo',
                    'warning',
                    'pink darken-2',
                    'red lighten-1',
                    'deep-purple accent-4',
                ],
                slides: [
                    'First-Agencies',
                    'Second-Agencies',
                    'Third-Agencies',
                    'Fourth-Agencies',
                    'Fifth-Agencies',
                ],

            }
        }
    }
</script>

<style scoped>

</style>