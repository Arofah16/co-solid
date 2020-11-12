<template>
  <v-app>
      <Testimoni/>
  </v-app>
</template>

<script>
import Testimoni from './views/Testimoni';

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
