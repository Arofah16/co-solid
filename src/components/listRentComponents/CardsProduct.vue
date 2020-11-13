<template>
  <v-row justify="start">
    <v-col cols="4" v-for="product in listProduct"
        :key="product.key">
      <v-card
        class="mx-auto"
        max-width="400"
        
      >
        <v-img
          class="white--text align-end"
          height="200px"
          src="@/assets/large_room.jpg"
        >
        </v-img>
          <v-card-title>{{ product.title }}</v-card-title>

        <v-card-subtitle class="pb-0">
          Rp. {{ product.price }} /2hr</v-card-subtitle
        >

        <v-card-text class="text--primary">
          <v-list class="transparent">
            <v-list-item
              v-for="(facility, index) in product.facilities"
              :key="index"
            >
              <v-list-item-title>{{ index }}</v-list-item-title>

              <v-list-item-icon>
                <v-icon>{{facility.icon}}</v-icon>
              </v-list-item-icon>

              <v-list-item-subtitle class="text-right">
                {{ facility.val }}
              </v-list-item-subtitle>
            </v-list-item>
          </v-list>
        </v-card-text>

        <v-card-actions >
          <v-btn  color="#005546" class="white--text mx-auto" block> Book </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    listProduct: [
      {
        id: 1,
        title: "Small Room",
        urlImg: "@/assets/small_room.jpg",
        price: "200.000",
        facilities: {
          capacity: {
            val: "5 - 10 person",
            icon: "mdi-account-group",
          },
          desert: {
            val: "Free drink",
            icon: "mdi-glass-cocktail",
          },
          Internet: {
            val: "20 mbps",
            icon: "mdi-lan-connect",
          },
        },
      },
      {
        id: 1,
        title: "Medium Room",
        urlImg: "@/assets/medium_room.jpg",
        price: "400.000",
        facilities: {
          capacity: {
            val: "10 - 15 person",
            icon: "mdi-account-group",
          },
          desert: {
            val: "Free drink",
            icon: "mdi-glass-cocktail",
          },
          Internet: {
            val: "30 mbps",
            icon: "mdi-lan-connect",
          },
        },
      },
      {
        id: 1,
        title: "Large Room",
        urlImg: "@/assets/large_room.jpg",
        price: "500.000",
        facilities: {
          capacity: {
            val: "15 - 25 person",
            icon: "mdi-account-group",
          },
          desert: {
            val: "Free drink",
            icon: "mdi-glass-cocktail",
          },
          Internet: {
            val: "50 mbps",
            icon: "mdi-lan-connect",
          },
        },
      },
    ],
  }),
  computed:{
    getImg(url){
      return require(url)
    }
  },
  methods: {
    getImgUrl(pic) {
      return require(pic);
    },
  },
};
</script>