<template>
  <div>
    <v-main>
      <Header></Header>
     <!-- <div style="background: #F3F4F5;">-->
     <MainContent />

    </v-main>
  </div>
</template>

<script>
import Navbar from "../components/Navbar";
import Header from "../components/Header";
import MainContent from "../components/MainContent";
export default {
  name: "Home",
  components: {
    Navbar, Header, MainContent
  }
}
</script>

<style scoped>

</style>