<template>
  <div>
    <div class="wave">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path fill="#f3f4f5" fill-opacity="1"
              d="M0,192L48,181.3C96,171,192,149,288,138.7C384,128,480,128,576,149.3C672,171,768,213,864,202.7C960,192,1056,128,1152,101.3C1248,75,1344,85,1392,90.7L1440,96L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path>
      </svg>
    </div>
    <div style="background: #F3F4F5; display: flex; justify-content: center;">
      <v-card class="info-card rounded-lg" color="#040D21">
        <v-container>
          <v-row justify="center">
            <v-col>
              <h1 class="title">Get the reputation of the whole world</h1>
            </v-col>
          </v-row>
        </v-container>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainContent"
}
</script>

<style scoped>
.wave > svg {
  display: block;
}
.title {
  font-size: 40px !important;
  background: -webkit-linear-gradient(-70deg,#a2facf,#64acff);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.info-card {
  width: 95%;
}
</style>