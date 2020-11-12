<template>
  <div>
    <center>
      <h1 color="grey darken-2"> Our Testimony</h1>
    </center>
    <v-container fluid>
      <div>
        <v-row justify="center" align="center">
          <v-col cols="6">
            <v-card color="#005546" outlined width="500" height="310">
              <v-list-item>
                <v-row justify="center">
                  <v-list-item-avatar size="70px">
                    <v-img height="80px" width="80px" rounded src="@/assets/mr.jpeg"></v-img>
                  </v-list-item-avatar>
                </v-row>
              </v-list-item>
              <v-card class="mx-auto mt-10" max-width="300" outlined>
                <v-card-subtitle>Been here for remote working. Perfect ambience for working, hangout with friends and
                  meeting. The coffee is also good, music is not too loud so you can enjoy your time perfectly.
                </v-card-subtitle>
              </v-card>
            </v-card>
          </v-col>
          <v-col cols="6">
            <v-card color="#005546" outlined width="500" height="310">
              <v-list-item>
                <v-row justify="center">
                  <v-list-item-avatar size="70px">
                    <v-img height="80px" width="80px" rounded src="@/assets/mrs.jpg"></v-img>
                  </v-list-item-avatar>
                </v-row>
              </v-list-item>
              <v-card class="mx-auto mt-10" max-width="300" outlined>
                <v-card-subtitle>Been here for remote working. Perfect ambience for working, hangout with friends and
                  meeting. The coffee is also good, music is not too loud so you can enjoy your time perfectly.
                </v-card-subtitle>
              </v-card>
            </v-card>
          </v-col>
        </v-row>
      </div>
      <div class="mt-16">
        <v-list-item-content>
          <p class="text-center b">Let’s work at workplace <br> of tomorrow</p>
        </v-list-item-content>
      </div>
      <div align="center" justify="space-around">
        <v-btn depressed color="#005546" class="white--text " height="45px" width='150px'>
          Book Now
        </v-btn>
      </div>



    </v-container>
  </div>
</template>
<script>
  export default {
    data: () => ({
    })
  }

</script>

<style scoped>
  .b {
    font-size: 60px;
    color: #616161;
    font-family: Arial, Helvetica, sans-serif;
  }
</style>