<template>
  <div>
    <Header1 />
    <v-main>
      <Section1 />
      <Section2 />
      <Section3 />
      <Section4 />
      <Section5 />
    </v-main>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header1 from "@/layouts/Header1";
import Section1 from "@/components/homeComponents/Section1";
import Section2 from "@/components/homeComponents/Section2";
import Section3 from "@/components/homeComponents/Section3";
import Section4 from "@/components/homeComponents/Section4";
import Section5 from "@/components/homeComponents/Section5";
import Footer from "@/layouts/Footer";
export default {
  name: "Home",
  components: {
    Header1,
    Section1,
    Section2,
    Section3,
    Section4,
    Section5,
    Footer,
  },
};
</script>

<style  >
.custom-color {
  color: #555555;
}
</style>