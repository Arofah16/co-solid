<template>
  <section class="pt-16 px-5" >
    <!-- <v-container fluid> -->
    <v-row>
      <v-col cols="12">
        <center>
          <h1 class="custom-color" style="font-size: 2em">Our Testimony</h1>
        </center>
      </v-col>
    </v-row>
    <v-row justify="space-between" align-content="space-around">
      <v-col cols="6" md="6" sm="12" xs="12">
        <v-card class="mx-auto" color="#005546" outlined width="500" height="310">
          <v-list-item>
            <v-row justify="center">
              <v-list-item-avatar size="90px">
                <v-img
                  height="80px"
                  width="80px"
                  rounded
                  src="@/assets/mr.jpeg"
                ></v-img>
              </v-list-item-avatar>
            </v-row>
          </v-list-item>
          <v-card class="mx-auto mt-8" max-width="300" outlined>
            <v-card-subtitle
              >Been here for remote working. Perfect ambience for working,
              hangout with friends and meeting. The coffee is also good, music
              is not too loud so you can enjoy your time perfectly.
            </v-card-subtitle>
          </v-card>
        </v-card>
      </v-col>

      <v-col cols="6" md="6" sm="12" xs="12">
        <v-card class="mx-auto" color="#005546" outlined width="500" height="310">
          <v-list-item>
            <v-row justify="center">
              <v-list-item-avatar size="90px">
                <v-img
                  height="80px"
                  width="80px"
                  rounded
                  src="@/assets/mrs.jpg"
                ></v-img>
              </v-list-item-avatar>
            </v-row>
          </v-list-item>
          <v-card class="mx-auto mt-8" max-width="300" outlined>
            <v-card-subtitle
              >Been here for remote working. Perfect ambience for working,
              hangout with friends and meeting. The coffee is also good, music
              is not too loud so you can enjoy your time perfectly.
            </v-card-subtitle>
          </v-card>
        </v-card>
      </v-col>
    </v-row>

    <!-- </v-container> -->
  </section>
</template>
<script>
export default {
  data: () => ({}),
};
</script>

<style scoped>
</style>