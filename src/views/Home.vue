<template>
  <div>
    <v-main>
      <Header></Header>
      <div class="wave">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
          <path fill="#f3f4f5" fill-opacity="1"
                d="M0,192L48,181.3C96,171,192,149,288,138.7C384,128,480,128,576,149.3C672,171,768,213,864,202.7C960,192,1056,128,1152,101.3C1248,75,1344,85,1392,90.7L1440,96L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path>
        </svg>
      </div>
      <div style="background: #F3F4F5;">
        <h1 class="title">Get the reputation of the whole world</h1>
      </div>
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
.wave > svg {
  display: block;
}

.title {
  background: linear-gradient(to bottom right, #9EF4CF, #5089BB);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 50px;
}
</style>