<template>
  <section >
      <v-app-bar
    :style="{ backgroundColor: change_color ? '#005546' : 'transparent' }"
    fixed
    flat
  >
    <v-toolbar-title>
      <v-img src="@/assets/logo_with_text.png"></v-img>
    </v-toolbar-title>

    <v-spacer></v-spacer>

    <v-btn text class="text-capitalize pr-1" color="white"> Reservasi </v-btn>

    <v-btn text class="text-capitalize pr-1" color="white"> Testimony </v-btn>

    <v-btn text class="text-capitalize pr-1" color="white"> Our Story </v-btn>
  </v-app-bar>
  </section>
</template>

<script>
export default {
  name: "Home",
  data: () => ({
    scrollPosition: null,
  }),
  computed: {
    change_color() {
      return this.scrollPosition > 200;
    },
  },
  methods: {
    updateScroll() {
      this.scrollPosition = window.scrollY;
    },
  },
  mounted() {
    window.addEventListener("scroll", this.updateScroll);
  },
};
</script>

<style scoped>
.change-color {
  background-color: red;
}
</style>