<template>
  <v-app>
    <Navbar/>
      <router-view/>

  </v-app>
</template>

<script>
import Home from "./views/Home";
import Navbar from "./components/Navbar";

export default {
  name: 'App',

  components: {
    Home, Navbar
  },

  data: () => ({
    //
  }),
};
</script>
