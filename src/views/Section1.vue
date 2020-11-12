<template>
    <div>
        <v-app-bar :style="{backgroundColor: (change_color)? '#005546': 'transparent'} "
        fixed color='rgba(255, 255, 255, 0)' elevate-on-scroll scroll-target="#section3">
            <v-toolbar-title>
                <v-img src="@/assets/logo_with_text.png"></v-img>
            </v-toolbar-title>

            <v-spacer></v-spacer>

            <v-btn text class="text-capitalize" color="white"> Reservasi </v-btn>

            <v-btn text class="text-capitalize" color="white"> Testimoni </v-btn>

            <v-btn text class="text-capitalize" color="white"> Our Story </v-btn>
        </v-app-bar>

        <!-- Sizes your content based upon application components -->
        <v-main>
            <!-- Hero section -->
            <section :style="{
            background:
              'linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),' +
              'url(' +
              require('@/assets/hero_bg.jpg') +
              ')',
            'background-position': 'center',
            'background-repeat': 'no-repeat',
            'background-size': 'cover',
            height: '100vh',
          }">
                <v-row style="align-items: center; height: 100%">
                    <v-col md="12" offset-md="4">
                        <h1 style="font-size: 3em" class="white--text">
                            Reimagine your <br />workspace
                        </h1>
                        <p class="white--text">
                            Whether you’re an established enterprise <br />
                            or a growing startup, discover flexible <br />
                            spaces and solutions to move <br />
                            your business forward.
                        </p>
                        <v-btn> BOOK NOW </v-btn>
                    </v-col>
                </v-row>
            </section>

            <section id="section3">
                <v-row justify="center" class="px-5">
                    <v-col cols='12'>
                        <v-card class="mx-auto" color="#005546" dark max-width="100%">
                            <v-card-actions>
                                <iframe width="100%" height="500vh" src="https://www.youtube.com/embed/3yAAGetLTF0"
                                    frameborder=""
                                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                    allowfullscreen></iframe>

                            </v-card-actions>
                        </v-card>
                    </v-col>
                </v-row>
                <div style="height:1000vh">

                </div>
            </section>
        </v-main>
        <v-footer dark padless>
            <v-card class="flex " color="#005546" flat tile>
                <v-card-title class="px-5">
                    <strong class="subheading">Get connected with us on social networks!</strong>

                    <v-spacer></v-spacer>

                    <v-btn v-for="icon in icons" :key="icon" class="mx-4" dark icon>
                        <v-icon size="24px">
                            {{ icon }}
                        </v-icon>
                    </v-btn>
                </v-card-title>

                <v-card-text class="py-2 black white--text text-center">
                    {{ new Date().getFullYear() }} — <strong>Arofah, Fahmi, Lambok</strong>
                </v-card-text>
            </v-card>
        </v-footer>
    </div>
</template>

<script>
    export default {
        name: 'Home',
        data: () => ({
            icons: [
                'mdi-facebook',
                'mdi-twitter',
                'mdi-linkedin',
                'mdi-instagram',
            ],
            scrollPosition: null
        }),
        computed:{
            change_color(){
            return this.scrollPosition >50
          }
        },
        methods: {
            updateScroll() {
                this.scrollPosition = window.scrollY
                console.log(this.scrollPosition)
            }
        },
        mounted() {
            window.addEventListener('scroll', this.updateScroll);
            
        }
    };
</script>

<style scoped>
 .change-color {
       background-color:red
   }
</style>