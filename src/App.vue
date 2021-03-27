<template>
  <v-app style="background: linear-gradient(to bottom right, #633CBA, #F46D71); font-family: Avenir, Helvetica, Arial, sans-serif;">
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
<style>

</style>