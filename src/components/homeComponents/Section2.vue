<template>
  <section class="px-5 pt-16">
    <!-- <v-container> -->
    <v-row  no-gutters>
      <v-col cols="6" md="6" sm="12" xs="12">
        <v-img width="100%" src="@/assets/one.png"></v-img>
      </v-col>
      <v-col cols="6" md="6" sm="12" xs="12" class="my-auto px-16">
        <div class="custom-color">
          <h1 style="font-size: 3em">
            Lorem Ipsum <br />
            dolor sir amet
          </h1>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit,<br />eiusmod
            tempor incididunt ut labore et dolore magna.<br />
            Ut enim ad minim veniam,
          </p>
        </div>
      </v-col>
    </v-row>
    <v-row class="pt-16" no-gutters>
      <v-col cols="6" md="6" sm="12" xs="12"  order="1" order-md="1" order-sm="2" order-xs="2">
        <div class="mx-16 custom-color">
          <h1 style="font-size: 3em">
            Lorem Ipsum <br />
            dolor sir amet
          </h1>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit,<br />eiusmod
            tempor incididunt ut labore et dolore magna.<br />
            Ut enim ad minim veniam,
          </p>
        </div>
      </v-col>

      <v-col cols="6" md="6" sm="12" xs="12" order="2" order-md="1" order-sm="1" order-xs="1">
        <v-img width="100%" src="@/assets/two.png"></v-img>
      </v-col>
    </v-row>
    <!-- </v-container> -->
  </section>
</template>
<script>
export default {
};
</script>

<style >

</style>
