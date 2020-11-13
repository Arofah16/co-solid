<template>
  <v-app>
      <Testimoni/>
      <Section2/>
  </v-app>
</template>

<script>
import Testimoni from './views/Testimoni';
import Section2 from './views/Section2';

export default {
  name: 'App',

  components: {
    Testimoni,
    Section2
  },

  data: () => ({
    //
  }),
};
</script>
