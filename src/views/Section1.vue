<template>
    <div>
      <v-app-bar
        absolute
        color="rgba(255, 255, 255, 0)"
        elevate-on-scroll
        scroll-target="#scrolling-techniques-7"
      >
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
        <section
          :style="{
            background:
              'linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),' +
              'url(' +
              require('@/assets/hero_bg.jpg') +
              ')',
            'background-position': 'center',
            'background-repeat': 'no-repeat',
            'background-size': 'cover',
            height: '100vh',
          }"
        >
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
        <!-- section 2 -->
        <section>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium
          laborum ipsam repudiandae maxime aperiam sequi sunt, corporis
          praesentium omnis dolor saepe facere commodi ut laboriosam voluptatibus,
          non suscipit, fugit iusto.
        </section>
        <!-- section 3 -->
        <section>
          <v-row>
            <v-col cols='12'>
              <video width="100%" height="100%">
                <source :src="videos" type="video/mp4" />
                Your browser does not support the video tag.
              </video>
            </v-col>
          </v-row>
        </section>
      </v-main>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Home',
    mounted() {
      // this.$refs.player.play();
    },
    data() {
      return {
        videos: '@/assets/videoplayback.mp4',
      };
    },
    components: {},
  };
  </script>
  