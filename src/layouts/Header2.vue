<template>
  <section>
    <v-app-bar
      color="#005546"
      
      flat
    >
      <router-link to="/">
        <v-toolbar-title>
          <v-img src="@/assets/logo_with_text.png"></v-img>
        </v-toolbar-title>
      </router-link>

      <v-spacer></v-spacer>

      <v-btn
        text
        class="text-capitalize "
        color="white"
        link
        to="/list-rent"
      >
        Reservasi
      </v-btn>

      <v-btn text class="text-capitalize " color="white"> Testimony </v-btn>

      <v-btn text class="text-capitalize " color="white"> Our Story </v-btn>
    </v-app-bar>
  </section>
</template>

<script>
export default {
};
</script>

<style scoped>
</style>