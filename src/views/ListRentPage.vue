<template>
  <div>
    <header-2 />
    <v-main>
      <v-container class="">
        <CardsProduct />
      </v-container>
      <Footer :isFixed="true"/>
    </v-main>
  </div>
</template>

<script>
import Header2 from '@/layouts/Header2'
import CardsProduct from '@/components/listRentComponents/CardsProduct'
import Footer from '@/layouts/Footer'
export default {
  components:{
    Header2,
    CardsProduct,
    Footer,
  }
}
</script>
