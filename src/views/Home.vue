<template>
  <div>
    <v-main>
      <Header></Header>
    </v-main>
  </div>
</template>

<script>
import Navbar from "../components/Navbar";
import Header from "../components/Header";
export default {
  name: "Home",
  components: {
    Navbar, Header
  }
}
</script>

<style scoped>

</style>