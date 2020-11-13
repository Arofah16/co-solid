<template>
  <div>
    <!-- <v-lazy
      v-model="isActive"
     :options="{
          threshold: .5
        }"
      transition="fade-transition"
      tag="div"
    > -->
    <v-footer dark padless>
      <v-card class="flex" color="#005546" flat tile>
        <v-card-title class="px-5">
          <strong class="subheading"
            >Get connected with us on social networks!</strong
          >

          <v-spacer></v-spacer>

          <v-btn v-for="icon in icons" :key="icon" class="mx-4" dark icon>
            <v-icon size="24px">
              {{ icon }}
            </v-icon>
          </v-btn>
        </v-card-title>

        <v-card-text class="py-2 black white--text text-center">
          {{ new Date().getFullYear() }} —
          <strong> &copy; by Praxis Academy</strong>
        </v-card-text>
      </v-card>
    </v-footer>
    <!-- </v-lazy> -->
  </div>
</template>

<script>
export default {
  data: () => ({
    isActive: false,
    icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
  }),
};
</script>

<style>
</style>